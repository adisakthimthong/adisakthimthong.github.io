<template lang="html">
  <div>
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <NuxtLink class="navbar-brand" :to="{ name: 'index' }"
          >BLONGBENZ</NuxtLink
        >
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse">
          <ul class="navbar-nav">
            <li class="nav-item">
              <NuxtLink class="nav-link" :to="{ name: 'posts' }"
                >Posts</NuxtLink
              >
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Menu 2</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#"
                >Menu 3</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.navbar {
  background-color: $color2;

  .navbar-brand, .nav-link{
    color: $color-white !important;
  }
}
</style>
