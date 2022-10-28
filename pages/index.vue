<template>
  <div>
    <Nav />
    <HomeCarousel :sale_items="sale_items" />
    <v-container>
      <h1 class="text-md-h4 text-h6"></h1>
      <br />
      <ProductSlider :webelements="webwlements" />
      <br/><br/><br/>
      <Newsletter />
    </v-container>
    <Footer />
    <ScrollTop />
  </div>
</template>

<script>

export default {
    async created() {
        this.sale_items = await this.$content("products").where({ onSale: true }).fetch();
        this.products = await this.$content("products").fetch();
        this.webelements = await this.$content("webelements").fetch();
    },
    data() {
        return {
            products: null,
            sale_items: null,
            webelements: null,
        };
    },
};
</script>

<style></style>