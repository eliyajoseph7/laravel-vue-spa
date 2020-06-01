<template>
    <div class="bg-light" id="learn">
        <div class="container">


            <!-- Section: Block Content -->
            <section class="dark-grey-text text-center">

                <h2 class="font-weight-bold">Start Learning</h2>
                <div class="divider mb-4 pb-2"></div>
                <p class="text-muted w-responsive mx-auto mb-5">Here you can find different tutorials which will help you to build and grow your programming skills. These tutorials are delivered in free of charge,
                    you only required to click on top-right on the navbar and <strong class="badge shadow badge-warning text-info">sign in</strong> or <strong class="badge shadow badge-warning text-info">sign up</strong>
                    if you don't have an account.
                </p>

                <!-- Grid row -->
                <div class="row">

                    <!-- Grid column -->
                    <div class="col-lg-4 col-md-12 mb-4">

                        <div class="view overlay rounded z-depth-1">
                        <img src="https://mdbootstrap.com/img/Photos/Others/images/58.jpg" class="img-fluid" alt="Sample project image">
                        <a>
                            <div class="mask rgba-white-slight"></div>
                        </a>
                        </div>

                        <div class="px-3 pt-3 mx-1 mt-1 pb-0">
                        <h4 class="font-weight-bold mt-1 mb-3">Creating Laravel App</h4>
                        <p class="text-muted">Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae.</p>
                        <a href="/create-laravel-app" class="btn btn-no1 btn-sm btn-rounded"><fa :icon="['fas', 'clone']" fixed-width /> View Tutorial</a>
                        </div>

                    </div>
                    <!-- Grid column -->

                    <!-- Grid column -->
                    <div class="col-lg-4 col-md-6 mb-4">

                        <div class="view overlay rounded z-depth-1">
                        <img src="https://mdbootstrap.com/img/Photos/Others/project4.jpg" class="img-fluid" alt="Sample project image">
                        <a>
                            <div class="mask rgba-white-slight"></div>
                        </a>
                        </div>

                        <div class="px-3 pt-3 mx-1 mt-1 pb-0">
                        <h4 class="font-weight-bold mt-1 mb-3">Basics of Vuejs</h4>
                        <p class="text-muted">Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae.</p>
                        <a href="#" class="btn btn-no2 btn-sm btn-rounded"><fa :icon="['fas', 'clone']" fixed-width /> View Tutorial</a>
                        </div>

                    </div>
                    <!-- Grid column -->

                    <!-- Grid column -->
                    <div class="col-lg-4 col-md-6 mb-4">

                        <div class="view overlay rounded z-depth-1">
                        <img src="https://mdbootstrap.com/img/Photos/Others/images/88.jpg" class="img-fluid" alt="Sample project image">
                        <a>
                            <div class="mask rgba-white-slight"></div>
                        </a>
                        </div>

                        <div class="px-3 pt-3 mx-1 mt-1 pb-0">
                        <h4 class="font-weight-bold mt-1 mb-3">Managing Django URL</h4>
                        <p class="text-muted">Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae.</p>
                        <a href="#" class="btn btn-no3 btn-sm "><fa :icon="['fas', 'clone']" fixed-width /> View Tutorial</a>
                        </div>

                    </div>
                    <!-- Grid column -->

                </div>
                <!-- Grid row -->
                <div class="pt-5">
                    <a class="btn btn-outline-primary btn-xl" href="#about">Find Out More</a>
                </div>
            </section>
            <!-- Section: Block Content -->


        </div>
    </div> 
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faClone } from '@fortawesome/free-solid-svg-icons'
library.add(faClone)
export default {
    name: 'Learning',
}
</script>

<style scoped>
    img:hover {
        transform: scale(1.1);
    }

    .btn-sm {
        border: none; /* Remove borders */
        color: white;
        padding: 0.5rem 2.0rem;
        font-size: 16px; 
        border-radius: 10rem;
    }
    .btn-no1 {
        background-color: brown;
    }
    .btn-no2 {
        background-color: #EE6600;
    }
    .btn-no3 {
        background-color: #F5AC05;
    }

    .btn-xl {
    padding: 1.25rem 2.25rem;
    font-size: 0.85rem;
    font-weight: 700;
    text-transform: uppercase;
    border: none;
    border-radius: 10rem;
}
</style>