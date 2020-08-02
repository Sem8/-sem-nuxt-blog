<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech memes</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbNail="https://i.chzbgr.com/full/9340631040/h7DD2A60F/find-out-that-your-peeler-is-several-versions-behind-and-they-dropped-support-for-carrots-in-43"
        title="Hello there!"
        previewText="This is my first post!"
      />
      <PostPreview
        id="2"
        thumbNail="https://miro.medium.com/max/1920/0*z1mm6izqSeDiKukb"
        title="Hello there - the second time!"
        previewText="This is my second post!"
      />
      <PostPreview
        id="3"
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
    PostPreview: PostPreview,
  },
}
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>

