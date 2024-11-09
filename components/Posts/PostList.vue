<template>
  <div class="post-list">
    <section class="featured-posts">
      <PostPreview
        id="1"
        title="First Post Title"
        text="This is the text of the first post."
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQCW-CGPywnnuY8e1TDNkYDlD-gFXPsjCfEQ&s"
      />
      <PostPreview
        id="2"
        title="Second Post Title"
        text="This is the text of the second post."
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQCW-CGPywnnuY8e1TDNkYDlD-gFXPsjCfEQ&s"
      />
      <PostPreview
        id="3"
        title="Third Post Title"
        text="This is the text of the third post."
        :thumbnail="postThumbnail"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview.vue";
import postThumbnail from "@/assets/images/post-thumbnail-image.png";
export default {
  components: {
    PostPreview,
  },
  data() {
    return {
      postThumbnail,
    };
  },
};
</script>

<style scoped>
.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
.post-list {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>