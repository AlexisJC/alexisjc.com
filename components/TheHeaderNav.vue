<template>
  <section class="hero is-primary">
    <!-- Hero head: will stick at the top -->
    <div class="hero-head"/>

    <!-- Hero content: will be in the middle -->
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title">
          Alexis CUELLAR
        </h1>
        <h2 class="subtitle">
          Développeur Web
        </h2>
      </div>
    </div>

    <!-- Hero footer: will stick at the bottom -->
    <div class="hero-foot">
      <nav class="tabs is-boxed">
        <div class="container">
          <ul>
            <nuxt-link 
              to="/" 
              tag="li"
              active-class="is-active"
              exact
            >
              <a>Résumé</a>
            </nuxt-link>
            <nuxt-link 
              to="/profil" 
              tag="li"
              active-class="is-active"
            >
              <a>Profil</a>
            </nuxt-link>
            <nuxt-link 
              to="/experiences" 
              tag="li"
              active-class="is-active"
            >
              <a>Expériences</a>
            </nuxt-link>
            <nuxt-link 
              to="/projects" 
              tag="li"
              active-class="is-active"
            >
              <a>Projets</a>
            </nuxt-link>
          </ul>
        </div>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style>
  li.is-active > a {
    color: #4fc08d!important;
  }
</style>

