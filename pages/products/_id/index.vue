<template lang="pug">
  div
    p Hi, this is product \#{{ $route.params.id }}
    button(@click='backProducts') Go back to main products page
</template>

<script>
export default {
  methods: {
    backProducts() {
      this.$router.push('/products')
    }
  }
}
</script>
