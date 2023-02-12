<template>
  <div class="container">
    <div class="row">
      <h4>Our Products</h4>
    </div>
    <div class="row">
      <div v-for="product of products" :key="product" class="col-md-6 col-xl-4 col-12 pt-3 d-flex">
        <ProductBox :product="product"></ProductBox>
      </div>
    </div>
  </div>
</template>
<script>
import ProductBox from "../../components/ProductBox";
export default {
  components: { ProductBox },
  props: ["products"],
};
</script>
