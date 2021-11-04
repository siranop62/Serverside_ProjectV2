<template>
    <div><hr>
        <h1> Show Order </h1>
            <p>id : {{ blog.id }} </p>
            <p>Title : {{ blog.title }} </p>
            <p>Order and address details : {{ blog.content }} </p>
            <p>Category : {{ blog.category }} </p>
            <p>Status : {{ blog.status }} </p>
            <p><b-button-group>
                <b-button variant="success" v-on:click="navigateTo('/blog/edit/'+blog.id)"> แก้ไขOrder </b-button>
                <b-button variant="dark" v-on:click="navigateTo('/blogs')"> กลับ </b-button>
            </b-button-group></p>
    </div>
</template>
<script>
import BlogsService from '@/services/BlogsService'
export default {
    data () {
        return { 
            blog: null
        }
    },
    async created () {
        try {
            let blogId = this.$route.params.blogId
            this.blog = (await BlogsService.show(blogId)).data
        } catch (error) {
            console.log (error)
        }
    },
    methods: {
       navigateTo (route) {
           this.$router.push(route)
       },
    }
}
</script>
<style scoped>
</style>