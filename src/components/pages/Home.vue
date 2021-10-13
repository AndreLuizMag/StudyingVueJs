<template>
  <Header />
  <main>
    <HomeTemplate />
  </main>
  <Footer />
</template>

<script>
import { Header, Footer } from '@/components/organisms'
import { HomeTemplate } from '@/components/templates'

export default {
  components: { Header, Footer, HomeTemplate }
}
</script>

<style lang="scss">
h1 {
  text-align: center;
  padding: 4rem 0 2rem 0;
}
</style>
