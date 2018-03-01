<template lang="pug">
div
  section.pt-8.text-center.h-32.intro.bg-cover.bg-center
    h1.font-hairline.text-white Get the latest tech news!

  section.p-4.container.mx-auto
    PostPreview(postTitle="Hello" previewText="This is a simple preview" postId="1" thumbnail="https://images.pexels.com/photos/904276/pexels-photo-904276.jpeg?w=1260&h=750&dpr=2&auto=compress&cs=tinysrgb")
    PostPreview(postTitle="Other Hello" previewText="Other little preview" postId="2" thumbnail="https://images.pexels.com/photos/902204/pexels-photo-902204.jpeg?w=1260&h=750&dpr=2&auto=compress&cs=tinysrgb")
    PostPreview(postTitle="Last hello" previewText="Last little preview" postId="3" thumbnail="https://images.pexels.com/photos/460200/pexels-photo-460200.jpeg?w=1260&h=750&dpr=2&auto=compress&cs=tinysrgb")
</template>

<script>
import PostPreview from '@/components/posts/PostPreview'

export default {
  components: {
    PostPreview
  }
}
</script>

<style scoped>
  .intro {
    background-image: url('~assets/images/background.jpeg');
  }
</style>

