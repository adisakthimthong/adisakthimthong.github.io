<template lang="html">
    <div class="card">
      <img
        src="https://picsum.photos/600/300/?image=25"
        class="card-img-top"
        alt="..."
      />
      <div class="card-body">
        <h5 class="card-title">{{ title }}</h5>
        <p class="card-text">
          {{ description }}
        </p>
        <NuxtLink
          class="btn btn-primary"
          :to="{ name: 'posts-slug', params: { slug: slug } }"
          >Read</NuxtLink
        >
      </div>
    </div>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      default: '',
    },
    description: {
      type: String,
      default: '',
    },
    slug: {
      type: String,
      default: '',
    },
  },
  mounted() {},
};
</script>
<style lang="scss"></style>
