<template>
  <NuxtLayout>
    <div
      ref="pagetop"
      class="flex-col items-center m-6 flxed"
    >
      <NuxtPage />
      <Footer />
    </div>
  </NuxtLayout>
  <button @click="scrollTo" class="fixed bottom-0 right-0 z-10 mb-5 mr-5">
    top
  </button>
</template>

<script setup>
  const pagetop = ref(null)

  function scrollTo() {
    pagetop.value.scrollIntoView({ behavior: 'smooth' })
  }
</script>
