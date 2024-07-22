<template>
  <div>
    <header>
      <h1>
        <NuxtLink to="/">Nuxt Shopping</NuxtLink>
      </h1>
    </header>
    <Nuxt></Nuxt>
  </div>
</template>

<script>
export default {
  layout: 'error',
  props: ['error'], // you can set a custom layout for the error page
}
</script>

<style lang="scss" scoped></style>
