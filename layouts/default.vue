<template>
  <div class="">
    <AppHeader></AppHeader>
    <nuxt></nuxt>
  </div>
</template>

<script>
import AppHeader from '../components/AppHeader.vue'
export default {
  components: { AppHeader },
}
</script>

<style scoped>
header {
  height: 60px;
  display: flex;
  align-items: center;
  padding: 0 0.5rem;
}
.logo {
  font-weight: 900;
}
.logo:visited {
  color: inherit;
}
</style>
