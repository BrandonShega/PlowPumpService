<template>
  <div class="home">
    <div class="cta">
      <img class="snow" alt="Vue logo" src="../assets/snow.jpg">
      <div class="info">
        <span>
          Snow season is upon us again.
          With snow on it's way, you need your
          plow in perfect working order.
          Here are the perfect kits for you do-it-yourselfers
          and rebuilds for those who need more.
          <br><br>
          Get your's now before it's too late!
        </span>
      </div>
    </div>
    <h1>Products</h1>
    <div class="products">
      <product-detail
        v-for="(product, index) in products"
        :product="product"
        :index="index"
        :key="product.id"
      ></product-detail>
    </div>
  </div>
</template>

<style lang="sass" scoped>
.home
  display: flex
  flex-direction: column

  .cta
    display: flex
    margin-bottom: 100px

  .snow
    width: 50%

  .info
    display: flex
    padding: 20px

    span
      margin: auto
      font-size: 16px

.products
  margin-top: 20px
  display: flex
  justify-content: space-between

</style>

<script>
import ProductDetail from '../components/ProductDetail'
import data from '../data/data'
export default {
  data: function () {
    return {
      products: data
    }
  },
  components: {
    ProductDetail
  }
}
</script>
