<template lang="html">
    <div>
         <b-card
            :title="title"
            img-src="https://picsum.photos/600/300/?image=25"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 20rem"
            class="mb-2"
        >
          <b-card-text>
            {{ description }}
          </b-card-text>

          <b-button
            :to="{ name: 'posts-slug', params: { slug: slug } }"
            variant="primary"
            >Go somewhere</b-button>
        </b-card>
    </div>
</template>
<script>
export default {
    props: {
        title: {
            type: String,
            default: ""
        },
        description:{
            type: String,
            default: ""
        },
        slug:{
            type: String,
            default: ""
        }
    },
    mounted(){
        
    }
}
</script>
<style lang="scss">
    
</style>