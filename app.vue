<template>
  <NuxtLayout>
    <div ref="pagetop"
      class="items-center p-6 m-6 border-8 flxed ex-col fiflex border-border rounded-3xl"
    >
      <Header />
      <NuxtPage />
      <Footer />
    </div>
  </NuxtLayout>
  <button @click="scrollTo" class="fixed bottom-0 right-0 z-10 mb-5 mr-5">Click me</button>
</template>

<script setup>
  const pagetop = ref(null)

  function scrollTo() {
    pagetop.value.scrollIntoView({ behavior: 'smooth' })
  }
</script>
