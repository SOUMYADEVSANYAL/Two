<template>
  <div class="admin-new-post-page">
    <section class="new-post-form">
      <AdminPostForm />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm.vue";
export default {
  layout: 'admin',
  components: {
    AdminPostForm,
  },
};
</script>

<style scoped>
/* .admin-new-post-page {
  position: relative;
  padding: 30px;
  left: 20%;
  width: 50%;
}
.new-post-form {
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