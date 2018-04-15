<template lang="pug">
  .container
    div
      p Hi, this is product \#{{ $route.params.id }}
      button(@click="$router.push('/products')") Go back to main products page
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  }
}
</script>
