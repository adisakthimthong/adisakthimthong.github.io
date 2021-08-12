<template lang="html">
    <div>
        <h1>{{post.title}}</h1>
        <p>{{post.description}}</p>
        <hr />
        <nuxt-content :document="post"></nuxt-content>
    </div>
</template>
<script>
export default {
    async asyncData({$content, params}) {
        const postData = await $content('posts', params.slug).fetch();
        return{
            post: postData,
        };
    }
}
</script>
<style lang="">
    
</style>