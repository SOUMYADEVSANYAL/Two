<template>
  <div class="admin-update-post-page">
    <section class="update-post-form">
      <AdminPostForm :loadedPost="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm.vue";
export default {
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: "Nick Wilde",
        title: "Loaded Post",
        thumbnailLink:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQCW-CGPywnnuY8e1TDNkYDlD-gFXPsjCfEQ&s",
        content: "The Content is not that important now.",
      },
    };
  },
};
</script>

<style scoped>
/* .admin-update-post-page {
  position: relative;
  padding: 30px;
  left: 20%;
  width: 50%;
}
.update-post-form {
  padding: 10px;
  color: aliceblue;
  border-radius: 10px;
  box-sizing: border-box;
  border: 1px solid black;
  background-image: url("~assets/images/post-thumbnail-image.png");
}*/
form {
  position: relative;
  top: 10%;
  left: 18%;
  width: 80%;
}
</style>