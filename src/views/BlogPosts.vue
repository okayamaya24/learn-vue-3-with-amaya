<template>
    <div class="blog-posts-layout">
        <aside class="blog-post-list">
            <BlogPostList></BlogPostList>
        </aside>
        <main class="blog-post-content">
            <router-view></router-view>
        </main>
    </div>
</template>

<script setup>
import BlogPostList from '@/Components/BlogPostList.vue'
</script>

<style lang="scss" scoped>
.blog-posts-layout {
    display: flex;
    gap: 1rem;

    .blog-post-list {
        flex: 0 0 25%
    }

    .blog-post-content {
        flex: 0 0 75%;
    }
}
</style>