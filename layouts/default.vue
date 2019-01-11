<template>
  <div>
    <TheHeaderNav />
    <section class="section">
      <nuxt/>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          Crée avec <v-external-link link="vuejs.org"><strong>Vue</strong></v-external-link>, stylisé par <v-external-link link="bulma.io"><strong>Bulma</strong></v-external-link>, 
          généré via <v-external-link link="nuxtjs.org"><strong>Nuxt</strong></v-external-link>, herbergé sur <v-external-link link="netlify.com"><strong>Netlify</strong></v-external-link>.
        </p>
        <div 
          class="columns is-mobile" 
          style="max-width: 500px; margin: auto;">
          <div class="column is-one-quarter">
            <figure class="image is-32x32">
              <img src="/vue_logo.png">
            </figure>
          </div>
          <div class="column is-one-quarter">
            <figure class="image is-32x32">
              <img src="/bulma_logo.png">
            </figure>
          </div>
          <div class="column is-one-quarter">
            <figure class="image is-32x32">
              <img src="/nuxt_logo.png">
            </figure>
          </div>
          <div class="column is-one-quarter">
            <figure class="image is-32x32">
              <img src="/netlify_logo.png">
            </figure>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import TheHeaderNav from '@/components/TheHeaderNav'
import vExternalLink from '@/components/v-external-link'

export default {
  components: {
    TheHeaderNav,
    vExternalLink
  }
}
</script>

<style>
  .hero.is-primary {
    background-color: #4fc08d !important;
  }
  span.is-primary {
    color: #4fc08d !important;
  }
  figure {
    margin: auto!important;
  }
</style>



