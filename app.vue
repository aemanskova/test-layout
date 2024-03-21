<template>
  <div class="wrapper">
    <Header />
    <PricesBlock />
    <UltraBlock></UltraBlock>
    <!-- <div style="height: 500px; background-color: white"></div> -->
    <WhiteSection />
    <Footer />
  </div>
</template>
<style lang="scss">
html,
body {
  padding: 0;
  margin: 0;
  border: 0;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  overflow-x: hidden;
  p,
  span,
  h1 {
    padding: 0;
    margin: 0;
  }
}
</style>
<script>
import MonochromeCards from "./components/MonochromeCards.vue";
export default {
  components: { MonochromeCards },
  head() {
    return {
      link: [
        { rel: "preconnect", href: "https://fonts.googleapis.com" },
        {
          rel: "preconnect",
          href: "https://fonts.gstatic.com",
          crossorigin: true,
        },
        {
          rel: "stylesheet",
          href: "https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap",
        },
      ],
    };
  },
};
</script>
