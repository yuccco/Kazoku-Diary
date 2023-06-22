<template>
  <h3 id="log" class="mb-4 text-3xl font-bold">運営日記</h3>
  <Carousel class="py-6 my-6 bg-white rounded-lg">
    <Slide v-for="blog in data?.contents" :key="blog.id">
      <div class="">
        <p class="text-lg font-bold">{{ blog.title }}</p>
        <p class="text-xs text-brownsub">
          {{ new Date(blog.publishedAt).toLocaleDateString() }}
        </p>
        <div class="mt-2 news" v-html="blog.body" />
      </div>
    </Slide>
    <template #addons>
      <Navigation />
      <Pagination />
    </template>
  </Carousel>
</template>

<script setup lang="ts">
  import 'vue3-carousel/dist/carousel.css'
  import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'

  import { Blog } from '~~/types/blog'
  const { data } = await useMicroCMSGetList<Blog>({
    endpoint: 'news'
  })
  console.log(data)
</script>
