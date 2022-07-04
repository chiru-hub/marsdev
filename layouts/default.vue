<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style>
body {
  background: rgb(2, 27, 121);
  background: linear-gradient(
    180deg,
    rgba(2, 27, 121, 1) 30%,
    rgba(5, 117, 230, 1) 100%
  );
}
.container {
  @apply max-w-screen-2xl mx-auto px-2;
}
</style>
