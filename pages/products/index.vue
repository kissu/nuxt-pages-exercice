<template lang="pug">
  div
    p Awesome product page huh ? :D
    p Pls enter the number of the product you're looking for

    input(type='text' v-model='productId')
    button(@click='submitProduct') Track product
</template>

<script>
export default {
  data() {
    return {
      productId: ''
    }
  },
  methods: {
    submitProduct() {
      this.$router.push('/products/' + this.productId)
    }
  }
}
</script>
