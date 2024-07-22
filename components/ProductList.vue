<template>
  <div>
    {{ products }}
  </div>
</template>

<script>
import axios from 'axios'
export default {
  async asyncData() {
    const response = await axios.get('http://localhost:3000/products')
    const prdoucts = response.data
    return { prdoucts }
  },
}
</script>

<style lang="scss" scoped></style>
