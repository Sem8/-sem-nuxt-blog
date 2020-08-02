<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: 'Sem',
        title: 'My awesome Post',
        content: 'Super amazing, thanks for that!',
        thumbnailLink: 'https://miro.medium.com/max/1920/0*z1mm6izqSeDiKukb',
      },
    }
  },
}
</script>