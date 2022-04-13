<script>
import ProjectComponent from "./ProjectComponent.vue"
export default {
    data() {
        return {
            posts: [
                { id: 1, content: '...', image: '/images/p1.jpg' },
                { id: 2, content: '...', image: '/images/p2.jpg' },
            ]
        };
    },
    components: { ProjectComponent }
}
</script>

<template>
    <div class="p-4 p-md-5 mb-4 rounded bg-light">
        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
            <ProjectComponent
                v-for="post in posts"
                v-bind:content="post.content"
                v-bind:image="post.image"
                v-bind:key="post.id"
            ></ProjectComponent>
        </div>
    </div>
</template>