<template>
  <div>
    <header>
      <h1>{{$route.name}}</h1>
      <NuxtLink to="/">HomePage</NuxtLink>
      <NuxtLink to="/main">MainPage</NuxtLink>
      <NuxtLink to="/product">Product Page</NuxtLink>
    </header>
    <Nuxt></Nuxt>
  </div>
</template>

<script>
export default {
    layout: 'error',
    props: ['error'] // you can set a custom layout for the error page
  }
</script>

<style lang="scss" scoped>

</style>