<template>
  <div class="product-detail">
    <img src="@/assets/placeholder.png" alt="">
    <h4 class="detail-title">{{ product.title }}</h4>
    <p class="detail-description">{{ product.description }}</p>
    <button class="detail-buy">Buy Now</button>
  </div>
</template>

<style lang="sass" scoped>
img
  width: 100%

.product-detail
  display: flex
  flex-direction: column
  padding: 20px
  align-items: center
  border: 1px solid #000
  border-radius: 5px
  margin: 0 10px

  &:first-child
    margin-left: 0

  &:last-child
    margin-right: 0

.detail-description
  flex: 1 0 auto

.detail-buy
  width: 100px
  border: none
  background: blue
  padding: 10px 20px
  color: white
  border-radius: 5px
  font-weight: bold
</style>

<script>
export default {
  props: ['product']
}
</script>
