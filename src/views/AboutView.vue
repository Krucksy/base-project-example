<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script>
import { useMeta } from 'vue-meta'
export default {
  name: "AboutView",
  setup () {
    useMeta({
      title: 'About page',
      description: 'Ceci est une description de la page about',
      htmlAttrs: { lang: 'fr', amp: true }
    })
  }
}
</script>


<style scoped lang=scss>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>