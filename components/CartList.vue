<template>
  <div class="list-wrapper">
    <ul>
      <li
        v-for="cart in $store.state.cartItems"
        :key="cart.id"
        class="list-item"
      >
        <img class="thumbnail" :src="cart.imageUrl" :alt="cart.name" />
        <div class="description">
          <p>{{ cart.name }}</p>
          <span>{{ cart.price }}</span>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
import { FETCH_CART_ITEMS } from '../store'

export default {
  async fetch() {
    await this.$store.displatch(FETCH_CART_ITEMS)
  },
}
</script>

<style scoped>
.list-wrapper {
  margin: 0.4rem 0;
}
.list-item {
  display: flex;
}
.thumbnail {
  width: 100px;
  height: 100px;
}
.description {
  padding: 2rem 1rem;
}
</style>
