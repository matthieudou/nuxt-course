<template lang="pug">
nuxt-link.no-underline.text-black.block.mb-4.shadow(:to="`/posts/${postId}`")
  article
    .w-full.h-32.bg-cover(:style="{backgroundImage: `url('${thumbnail}')`}")
    .bg-grey-light.p-4
      h1.font-hairline.mb-2 {{postTitle}}
      p {{previewText}}
</template>

<script>
export default {
  props: {
    postId: {
      type: String,
      required: true
    },
    thumbnail: {
      type: String,
      required: true
    },
    postTitle: {
      type: String,
      required: true
    },
    previewText: {
      type: String,
      required: true
    }
  }
}
</script>
