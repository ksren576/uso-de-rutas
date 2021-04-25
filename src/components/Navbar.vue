<template>
  <nav class="navbar navbar-expand-sm navbar-light">
    <div class="container">
      <router-link class="navbar-brand" to="/">v8</router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="containercollapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <router-link to="/" v-slot="{ href, navigate, isExactActive }" custom>
            <li :class="['nav-item', isExactActive && 'active']">
              <a :href="href" @click="navigate" class="nav-link" to="/">Home</a>
            </li>
          </router-link>
          <router-link to="/post/1" v-slot="{ href, navigate, isExactActive }" custom>
            <li :class="['nav-item', isExactActive && 'active']">
              <a :href="href" @click="navigate" class="nav-link" to="/">Artículos</a>
            </li>
          </router-link>
          <router-link to="/contact" v-slot="{ href, navigate, isExactActive }" custom>
            <li :class="['nav-item', isExactActive && 'active']">
              <a :href="href" @click="navigate" class="nav-link" to="/">Contacto</a>
            </li>
          </router-link>
          <router-link to="/about" v-slot="{ href, navigate, isExactActive }" custom>
            <li :class="['nav-item', isExactActive && 'active']">
              <a :href="href" @click="navigate" class="nav-link" to="/">Sobre mí</a>
            </li>
          </router-link>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
nav {
  background-color: #FFCC33;
}
</style>