<template>
  <div class="container">
    <h1 class="list-title">Cart Page</h1>
    <CartList></CartList>
    <div class="extra-panel">
      <button>구매하기</button>
    </div>
  </div>
</template>

<script>
import CartList from '../components/CartList.vue'
// import { FETCH_CART_ITEMS } from '../store'

export default {
  components: { CartList },
  // async asyncData({ store }) {
  //   await store.dispatch(FETCH_CART_ITEMS)
  // },
  // computed: {
  //   carts() {
  //     return this.$store.state.cartItems
  //   },
  // },
}
</script>

<style scoped>
.container {
  margin: 2rem 10rem;
}
.list-title {
  font-weight: 700;
  font-size: 1.4rem;
}
.extra-panel {
  text-align: right;
  padding: 0.2rem 0;
}
</style>
