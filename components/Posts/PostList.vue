<template>
     <section class="featured-posts">
      <PostPreview
        id="1"
        :isAdmin='isAdmin'
        thumbnail="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/Image_created_with_a_mobile_phone.png/220px-Image_created_with_a_mobile_phone.png"
        title="iPhone Photos"
        previewText="Hey guys, I've been feeling inspired"
      />
      <PostPreview
        id="2"
        :isAdmin='isAdmin'
        thumbnail="https://cdn5.vectorstock.com/i/1000x1000/21/69/single-cartoon-diary-on-white-background-vector-29562169.jpg"
        title="Dear Dairy"
        previewText="Hey guys, welcome to another episode"
      />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
      isAdmin: {
          type: Boolean,
          default: false
      }
  }
}
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
</style>