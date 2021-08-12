<template lang="html">
    <div>
        <b-row>
      <b-col v-for="post in posts" :key="post.slug">
        <Card 
          :title="post.title"
          :description="post.description"
          :slug="post.slug"
          ></Card>
      </b-col>
    </b-row>
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
}
</script>
<style lang="">
    
</style>