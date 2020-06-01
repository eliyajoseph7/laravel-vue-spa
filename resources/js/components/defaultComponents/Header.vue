<template>
  <header nativeOnScroll={this.handleScroll} :class="{'header': scrl}">

    <!-- Full Page Intro -->
    <div class="view grey lighten-3">
      <!-- Mask & flexbox options-->
      <div class="mask">
        <!-- Content -->
        <div class="container h-100">
          <!--Grid row-->
          <div class="row align-items-center h-100">
            <!--Grid column-->
            <div class="col-md-6">
              <h1 class="mb-4">Find the <span class="text-warning">best programming</span><br><span class="cyan-text">tips</span> and tutorials.</h1>
              <p class="mb-4 pb-2 dark-grey-text">Welcome to <strong class="text-info">Good Morning </strong> blog, here you will get to learn some different programming
               tips that will help you to improve your programming skills.</p>
              <a href="#learn" type="button" class="btn btn-primary btn-md ml-md-0">Get started</a>
              <!-- <button type="button" class="btn btn-md">Get started</button> -->
            </div>
            <!--Grid column-->
        
            <!--Grid column-->
            <div class="col-md-6">
              <img src="https://mdbootstrap.com/img/illustrations/hiker-man-colour.svg" alt="" class="img-fluid">
            </div>
            <!--Grid column-->
          </div>
          <!--Grid row-->
        </div>
        <!-- Content -->
      </div>
      <!-- Mask & flexbox options-->
    </div>
    <!-- Full Page Intro -->
    
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
    return {
      scrl: false
    }
  },
  methods: {
    handleScroll (event) {
      let st = window.scrollY
      if(st > 100){
        this.scrl = true
      }else{
        this.scrl = false
      }
    }
  },
  created () {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  }
}
</script>

<style scoped>
header {
  position: fixed;
  top: 60px;
  left: 10%;
  
}

.header{
  z-index: -1;
}

.btn-md {
    border: none; /* Remove borders */
    color: white;
    padding: 0.5rem 2.0rem;
    font-size: 16px; 
    border-radius: 10rem;
}
</style>