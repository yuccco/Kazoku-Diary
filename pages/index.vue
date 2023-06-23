<template>
  <div class="w-full mx-auto lg:px-12">
    <div class="flex items-end justify-center gap-3 mt-24 mb-24">
      <div class="flex justify-center w-1/5">
        <img src="~/assets/img/main_cat01.png" alt="ごきげんさん" width="250" />
      </div>
      <div class="flex flex-col items-center justify-center">
        <h1 class="mb-6 text-4xl text-center">
          <img src="~/assets/img/logo.svg" alt="家族ダイアリー" width="630" />
        </h1>
        <p class="mt-5 leading-9 text-center text-brownsub">
          家族や友達や恋人など、仲がいい人たちで交換日記を書こう！<br />
          日々のできごとを写真付きで投稿してシェアできる<br />
          シンプルな日記アプリです。<br />
          みんなで今日あったできごとを共有しあって日常のできごとを語り合いましょう！
        </p>
        <div class="flex flex-col mt-12 md:flex-row">
          <NuxtLink
            class="px-8 py-3 rounded-full p text-cream bg-brown hover:bg-brownsub hover:scale-105 hover:drop-shadow-xl hover:-rotate-2"
            to="https://apps.apple.com/jp/app/%E5%AE%B6%E6%97%8F%E3%83%80%E3%82%A4%E3%82%A2%E3%83%AA%E3%83%BC-%E4%BA%A4%E6%8F%9B%E6%97%A5%E8%A8%98%E3%82%A2%E3%83%97%E3%83%AA/id1528947553"
            target="_blank"
            >iPhone版</NuxtLink
          >
          <NuxtLink
            class="px-8 py-3 mt-2 ml-0 rounded-full p text-cream bg-brown hover:bg-brownsub hover:scale-105 hover:drop-shadow-xl md:ml-4 md:mt-0 hover:-rotate-2"
            to="https://play.google.com/store/apps/details?id=com.sekky.kibunya&hl=en_US"
            target="_blank"
            >Android版</NuxtLink
          >
        </div>
      </div>
      <div class="flex justify-center w-1/5">
        <img src="~/assets/img/main_cat02.png" alt="さいこうさん" width="230" />
      </div>
    </div>

    <div id="feather" class="mb-24">
      <h2 class="flex px-6 py-4 bg-sand rounded-[40px] justify-start items-center gap-3"><img src="~/assets/img/ashiato.svg" alt="" width="22" /><span class="text-lg font-bold leading-9 text-brown">アプリの特徴</span></h2>
    </div>

    <News />
  </div>
</template>
