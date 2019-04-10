<template>
  <div>
    <my-header />
    <nuxt />
  </div>
</template>

<script>
  import MyHeader from '~/components/Header.vue'
  export default {
    name: 'navbarFooterLess',
    components: {
      MyHeader
    }
  }
</script>

<style>
</style>