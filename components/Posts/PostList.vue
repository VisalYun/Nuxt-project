<template>
    <section class="post-list">
        <PostPreview 
            id="1"
            :is-admin="isAdmin"
            thumbnail="https://i.imgur.com/fLk1pxe.jpg"
            title="Nigga caught kissing!"
            previewText="Everyone are so fin with these 2 niggas!"
        />
        <PostPreview 
            id="2"
            thumbnail="https://i.imgur.com/fLk1pxe.jpg"
            title="Nigga caught kissing again!"
            previewText="Everyone are so fin with these 2 niggas again!"
        />
        <PostPreview 
            id="3"
            thumbnail="https://i.imgur.com/fLk1pxe.jpg"
            title="Again and again!!! Nigga caught kissing!"
            previewText="These 2 niggas make everyone fin again and again!"
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
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>