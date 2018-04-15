<template lang="pug">
  div
    p Hi, this is product \#{{ $route.params.id }}
    button(@click="$router.push('/products')") Go back to main products page
</template>
