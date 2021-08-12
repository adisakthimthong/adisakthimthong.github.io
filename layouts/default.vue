<template lang="html">
  <div class="content-wrapper">
    <Topbar></Topbar>
    <div class="container py-5">
      <Nuxt></Nuxt>
    </div>
  </div>
</template>
<script>
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap';
export default {};
</script>
<style lang="scss">
.content-wrapper{
  background-color: rgba($color10, .7);
  min-height: 100vh;
}
</style>
