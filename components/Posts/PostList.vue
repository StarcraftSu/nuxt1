<template>
    <section class="post-list">
        <post-preview 
            id="1"
            :is-admin="isAdmin"
            title="Hello there"
            previewText="This is my first post"
        ></post-preview>
    </section>
</template> 
<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  },
  props:{
      isAdmin:{
          type:Boolean,
          default:false
      }
  }
}
</script>
<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
