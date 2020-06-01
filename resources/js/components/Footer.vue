<template>
  <div>
      <!-- Footer -->
<footer class="footer">

  <!-- Footer Elements -->
  <div class="container">
    <div class="row">
      <div class="col-md-4 p-3">
        
        <ul>
          <h2>Contact us</h2>
          <li><a href="mailto:exaveryeliya20@gmail.com">exaveryeliya20@gmail.com</a></li>
          <li>33335, Sam Nujoma road</li>
          <li>University of Dar es Salaam</li>
          <li>Tanzania.</li>
        </ul>
      </div>
      <div class="col-md-4 p-3">
        
        <ul>
          <h2 class="text-center">Faith in God</h2>
          <li><iframe width="100%" height="200" src="https://www.youtube.com/embed/UO_sRwcfVqI" frameborder="0" 
              allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></li>
        </ul>
      </div>
      <div class="col-md-4 p-3">
        <h2 class="text-center">Around the web</h2>
        <ul class="flex">
          <li><a href="#" target="_blank"><fa :icon="['fab', 'facebook']" pulse size="3x" :style="{ color: 'white' }" /></a></li>
          <li><a href="https://twitter.com/eliya_Joseph20" target="_blank"><fa :icon="['fab', 'twitter']" spin size="3x" :style="{ color: 'white' }" /></a></li>
          <li><a href="https://github.com/eliyajoseph7" target="_blank"><fa :icon="['fab', 'github']" spin size="3x" :style="{ color: 'white' }" /></a></li>
          <li><a href="#" target="_blank"><fa :icon="['fab', 'instagram']" pulse size="3x" :style="{ color: 'white' }" /></a></li>
        </ul>
      </div>
    </div>
  
  </div>
  <!-- Footer Elements -->
  <hr />
  <h1 class="text-center">We're warmely <strong class="text-warning">Welcoming</strong> you!</h1>
  <p class="text-center">Subscribe to get more news from us!.</p>
  <div class="flex-container">
    <input type="text" name="email">
    <a href="#" class="btn btn-primary">Subscribe</a>
  </div>
</footer>
<!-- Footer -->
  <!-- Copyright -->
  <div class="footer-copyright text-center py-3">© 2020 Copyright:
    <a href="#"> Good Morning</a>
  </div>
  <!-- Copyright -->
  </div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFacebook, faTwitter, faGithub, faInstagram } from '@fortawesome/free-brands-svg-icons'

library.add(
    faFacebook, faTwitter, faGithub, faInstagram
)
export default {
    name: "Footer"
}
</script>

<style>
    .footer {
        background-color: #1C2331;
        padding: 3rem;
        color: blanchedalmond;
    }
    .footer ul li {
        list-style-type: none;
    }

    .flex-container{
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
    }
    .flex-container input{
        width: 300px;
        margin: 1px 2px;
    }
    .footer-copyright {
        background-color: #161C27;
        color: #fff;
    }
    

    hr {
        border-top: 3px solid #2A6481;
    }

    .flex {
      display: flex;
      flex-flow: row wrap;
      justify-content: flex-start;
    }
    .flex li a{
      padding: 5px;
    }
</style>