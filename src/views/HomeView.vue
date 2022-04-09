<template>
  <main>
    <TheWelcome />
  </main>
</template>

<script>
import TheWelcome from '@/components/TheWelcome.vue'
import { useMeta } from 'vue-meta'

export default {
  name: "HomeView",
  components: {
    TheWelcome
  },
  setup () {
    useMeta({
      title: 'Home page',
      description: "Ceci est une description de la page d'accueil",
      htmlAttrs: { lang: 'fr', amp: true }
    })
  }
}
</script>

<style scoped lang=scss>

</style>