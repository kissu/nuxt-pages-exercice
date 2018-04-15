<template lang="pug">
  .container
    div
      yolo
      p Hi, this is product \#{{ $route.params.id }}
      button(@click="$router.push('/products')") Go back to main products page
</template>

<script>
import yolo from '~/components/yolo'

export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  },
  layout: 'products',
  components: {
    yolo
  }
}
</script>
