<template>
  <div class="posts-page">
    <section class="intro">
      <h1>Get the latest tech memes</h1>
    </section>
    <section class="post-list">
      <PostPreview
        id="1"
        :is-admin="isAdmin"
        thumbNail="https://i.chzbgr.com/full/9340631040/h7DD2A60F/find-out-that-your-peeler-is-several-versions-behind-and-they-dropped-support-for-carrots-in-43"
        title="Hello there!"
        previewText="This is my first post!"
      />
      <PostPreview
        id="2"
        :is-admin="isAdmin"
        thumbNail="https://miro.medium.com/max/1920/0*z1mm6izqSeDiKukb"
        title="Hello there - the second time!"
        previewText="This is my second post!"
      />
      <PostPreview
        id="3"
        :is-admin="isAdmin"
        thumbNail="https://i.chzbgr.com/full/9340629504/h5E49874A/distracted-boyfriend-meme"
        title="Hi!"
        previewText="This is my third post!"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview,
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