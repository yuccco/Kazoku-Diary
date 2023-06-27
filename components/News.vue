<template>
  <h2
    class="flex px-6 py-4 bg-sand rounded-[40px] justify-start items-center gap-3 mb-10"
  >
    <img src="~/assets/img/ashiato.svg" alt="" width="22" /><span
      class="text-2xl font-bold leading-9 text-brown"
      >かいはつ日記</span
    >
  </h2>
  <div class="flex flex-col px-0 mb-10 md:px-10">
    <Carousel class="mb-6 border-border rounded-[20px]">
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
  </div>
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
