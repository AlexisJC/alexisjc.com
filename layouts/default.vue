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
 .is-primary {
   background-color: #4fc08d !important;
 }
</style>



