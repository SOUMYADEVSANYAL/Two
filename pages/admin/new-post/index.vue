<template>
  <div class="admin-new-post-page">
    <section class="new-post-form">
      <form @submit.prevent="onSave">
        <AppControlInput v-model="editedPost.author"
          >Author Name</AppControlInput
        >

        <AppControlInput v-model="editedPost.title">Title</AppControlInput>

        <AppControlInput v-model="editedPost.thumbnailLink"
          >Thumbnail Link</AppControlInput
        >

        <AppControlInput control-type="textarea" v-model="editedPost.content"
          >Content</AppControlInput
        >

        <AppButton type="submit">Save</AppButton>

        <AppButton
          type="button"
          style="margin-left: 10px"
          btn-style="cancel"
          @click="onCancel"
          >Cancel</AppButton
        >
      </form>
    </section>
  </div>
</template>

<script>
import AppControlInput from "@/components/UI/AppControlInput.vue";
import AppButton from "@/components/UI/AppButton.vue";
export default {
  components: {
    AppControlInput,
    AppButton,
  },
  data() {
    return {
      editedPost: {
        author: "",
        title: "",
        thumbnailLink: "",
        content: "",
      },
    };
  },
  methods: {
    onSave() {
      console.log(this.editedPost);
    },
    onCancel() {
      this.$router.push("/admin");
    },
  },
};
</script>

<style>
.admin-new-post-page {
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
}
form {
  position: relative;
  top: 10%;
  left: 18%;
  width: 80%;
}
</style>