<template>
  <div>
    <div class="top-left">
      <!-- <template>
        {{title}}
      </template> -->
    </div>
    <!-- <div class="top-right links">
      <template v-if="authenticated">
        <router-link :to="{ name: 'home' }">
          {{ $t('home') }}
        </router-link>
      </template>
      <template v-else>
        <router-link :to="{ name: 'login' }">
          {{ $t('login') }}
        </router-link>
        <router-link :to="{ name: 'register' }">
          {{ $t('register') }}
        </router-link>
      </template>
    </div> -->
    <DefaultView />
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import DefaultView from '../components/DefaultView'
export default {
  layout: 'custom',

  components: {
    DefaultView
  },

  metaInfo () {
    return { title: this.$t('home') }
  },

  data: () => ({
    title: window.config.appName
  }),

  computed: mapGetters({
    authenticated: 'auth/check'
  })
}
</script>

<style scoped>
.top-right {
  position: absolute;
  right: 10px;
  top: 18px;
}
.top-left {
  position: absolute;
  left: 5%;
  top: 18px;
  right: 80%;
  font-size: 30px;
}

.title {
  font-size: 85px;
}
</style>
