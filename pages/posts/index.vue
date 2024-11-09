<template>
  <PostList :isAdmin="false"/>
</template>

<script>
import PostList from "@/components/Posts/PostList.vue";

export default {
  components: {
    PostList,
  },
};
</script>

<style scoped>
</style>