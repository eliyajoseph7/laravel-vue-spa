<template>
    <div>

      <!-- Main navigation -->
      <div class="start">
        <Header />
      
      </div> 
      <div style="margin-top: 450px; background-color: #fff"> 
          <Projects />
          <Learning />
        
        <div class="container mt-5">


          <!--Section: Content-->
          <section class="dark-grey-text pb-5">

            <!-- Section heading -->
            <h2 class="text-center font-weight-bold">Recent posts</h2>
            <div class="divider mb-4 pb-2"></div>
            <!-- Section description -->
            <p class="text-center mx-auto w-responsive mb-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit, error amet numquam iure provident voluptate esse quasi, veritatis totam voluptas nostrum quisquam eum porro a pariatur veniam.</p>

            <!-- Grid row -->
            <div class="row align-items-center">

              <!-- Grid column -->
              <div class="col-lg-5">

                <!-- Featured image -->
                <div class="view overlay rounded z-depth-2 mb-lg-0 mb-4">
                  <img class="img-fluid" src="https://mdbootstrap.com/img/Photos/Others/img%20(27).jpg" alt="Sample image">
                  <a>
                    <div class="mask rgba-white-slight"></div>
                  </a>
                </div>

              </div>
              <!-- Grid column -->

              <!-- Grid column -->
              <div class="col-lg-7">

                <!-- Category -->
                <a href="#!" class="green-text">
                  <h6 class="font-weight-bold mb-3"><i class="fas fa-utensils pr-2"></i>Food</h6>
                </a>
                <!-- Post title -->
                <h4 class="font-weight-bold mb-3"><strong>Title of the news</strong></h4>
                <!-- Excerpt -->
                <p>Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime
                  placeat facere possimus, omnis voluptas assumenda est, omnis dolor repellendus et aut officiis debitis.</p>
                <!-- Post data -->
                <p>by <a><strong>Carine Fox</strong></a>, 19/08/2018</p>
                <!-- Read more button -->
                <a class="btn btn-success btn-md btn-rounded mx-0">Read more</a>

              </div>
              <!-- Grid column -->

            </div>
            <!-- Grid row -->

            <!-- <hr class="my-5"> -->
            
          </section>
          <!--Section: Content-->


        </div>

      </div>
      <Footer />

    </div>
</template>

<script>
import Header from './defaultComponents/Header'
import Projects from './defaultComponents/Projects'
import Learning from './defaultComponents/Learning'
import Footer from './Footer'
export default {
  name: "DefaultView",
  components: {
    Header,
    Projects,
    Learning,
    Footer
  },
  
};
</script>

<style>
.start {
  background-color: aliceblue;
}

h2 {
  padding-top: 5rem;
}
.divider {
  border-top: 3px solid rgb(245, 11, 11);
  width: 100px;
  margin: auto;
}
/* Darker background on mouse-over */
    .btn:hover {
    background-color: RoyalBlue;
    }

    
</style>

