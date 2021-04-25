<template>
  <div>
    <hr />
    <div class="row">
      <div class="col">
        <div class="card mb-3">
          <img src="@/assets/img/home-bg.jpg" alt="Blazer" />
          <div class="card-body">
            <h5 class="card-title">
              Chevrolet presenta la totalmente nueva Blazer
            </h5>
            <p class="card-text">
              Llega como la primera SUV deportiva de la marca.
            </p>
            <router-link to="/post/1" class="card-link">Ver más...</router-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
