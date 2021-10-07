<template>
  <Header />
  <main>
    <h1>Home</h1>
  </main>
  <Footer />
</template>

<script>
import Header from "./components/Header/Header";
import Footer from "./components/Footer/Footer";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>
