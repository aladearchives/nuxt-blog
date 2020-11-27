<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>

import AdminPostForm from '../../../components/Admin/AdminPostForm'
export default {
  layout: admin,
    components: {
        AdminPostForm
    },
    data() {
        return {
            loadedPost: {
                author: 'Tosin',
                title: 'My Introduction',
                content: 'I just want to rant about things I find interesting',
                thumbnailLink: "https://cdn5.vectorstock.com/i/1000x1000/21/69/single-cartoon-diary-on-white-background-vector-29562169.jpg"
            }
        }
    }
}
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>