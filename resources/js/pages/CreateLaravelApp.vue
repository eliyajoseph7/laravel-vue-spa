<template>
    <div>
        <LaravelStart />
        <Footer />
    </div>
  
  
</template>

<script>
import LaravelStart from '../components/Learnings/LaravelStart'
import Footer from '../components/Footer'
export default {
    layout: "custom",
    components: {
        LaravelStart,
        Footer
    }

}
</script>

<style>

</style>