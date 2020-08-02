<template>
  <nuxt-link :to="'/posts/' + 1" class="post-preview">
    <article>
      <div
        class="post-thumbnail"
        style="background-image: url('https://i.chzbgr.com/full/9340631040/h7DD2A60F/find-out-that-your-peeler-is-several-versions-behind-and-they-dropped-support-for-carrots-in-43')"
      ></div>
      <div class="post-content">
        <h1>Post Title 1</h1>
        <p>Preview Text 1</p>
      </div>
    </article>
  </nuxt-link>
</template>

<style scoped>
.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: #ccc;
}
</style>