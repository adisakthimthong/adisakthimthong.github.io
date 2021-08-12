<template lang="html">
  <div>
    <h1>Posts</h1>
    <div class="row row-cols-1 row-cols-md-3 g-4">
      <div v-for="post in posts" :key="post.slug" class="col">
        <Card
          :title="post.title"
          :description="post.description"
          :slug="post.slug"
        ></Card>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  async asyncData({ $content }) {
    const postsData = await $content('posts').fetch();
    return {
      posts: postsData,
    };
  },
};
</script>
<style lang=""></style>
