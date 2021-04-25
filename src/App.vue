<template>
  <div id="app">
    <!-- CONTENIDO PARA LA VISTA DE PORTADA -->
    <Navbar />
    <header
      class="masthead"
    >
      <div class="overlay"></div>
      <div class="container">
        <div class="row">
          <div class="col mx-auto">
            <div class="site-heading">
              <h1 class="text-center">V8</h1>
              <h4 class="text-center">Noticias y reseñas de automóviles</h4>
            </div>
          </div>
        </div>
      </div>
    </header>
    <div class="container"><router-view /></div>
    <footer>
      <div class="container">
        <hr>
        <div class="row">
          <div class="col-auto mx-auto">
            <ul class="list-inline text-center">
              <li class="list-inline-item">
                <span class="fa-stack fa-lg"
                  ><i class="fa fa-circle fa-stack-2x"></i
                  ><i class="fa fa-twitter fa-stack-1x fa-inverse"></i
                ></span>
              </li>
              <li class="list-inline-item">
                <span class="fa-stack fa-lg"
                  ><i class="fa fa-circle fa-stack-2x"></i
                  ><i class="fa fa-facebook fa-stack-1x fa-inverse"></i
                ></span>
              </li>
              <li class="list-inline-item">
                <span class="fa-stack fa-lg"
                  ><i class="fa fa-circle fa-stack-2x"></i
                  ><i class="fa fa-github fa-stack-1x fa-inverse"></i
                ></span>
              </li>
            </ul>
            <p class="text-muted copyright text-center">Copyright V8 - 2018</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.min.css";
import Navbar from './components/Navbar';

export default {
  name: "App",
  components: {
    Navbar,
  },
};
</script>
