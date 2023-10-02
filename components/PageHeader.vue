<template>
<main class="background">
  <h1>Hello</h1>
</main>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
  .background{
   background: url('@/assets/img/background.jpg');
   background-repeat: no-repeat;
   background-size: cover;
  }
</style>
