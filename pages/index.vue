<template>
  <div class="w-full lg:w-[1024px] lg:px-12 mx-auto">
    <div class="flex flex-col items-center justify-center mt-20 mb-40">
      <h2 class="mb-5 text-4xl text-center">
        家族ダイアリー<br class="md:hidden" /><span class="text-lg"
          >〜交換日記アプリ〜
        </span>
      </h2>
      <h3 class="mb-5 text-brownsub">家族や友人と秘密の交換日記を楽しもう</h3>
      <img src="~/assets/img/appicon.png" alt="" width="300" />
      <p class="mt-5 text-center">
        家族や友達や恋人と交換日記を書こう！<br />
        日々のできごとを写真付きで投稿してシェアできます。<br />
        みんなで今日あったできごとを共有し合って、日常のできごとを語り合いましょう。
      </p>
      <div class="flex flex-col mt-5 md:flex-row">
        <NuxtLink
          class="px-5 py-4 rounded-full p text-cream bg-brown hover:bg-brownsub hover:scale-105 hover:drop-shadow-xl hover:-rotate-2"
          to="https://apps.apple.com/jp/app/%E5%AE%B6%E6%97%8F%E3%83%80%E3%82%A4%E3%82%A2%E3%83%AA%E3%83%BC-%E4%BA%A4%E6%8F%9B%E6%97%A5%E8%A8%98%E3%82%A2%E3%83%97%E3%83%AA/id1528947553"
          target="_blank"
          >iOSダウンロード</NuxtLink
        >
        <NuxtLink
          class="px-5 py-4 mt-2 ml-0 rounded-full p text-cream bg-brown hover:bg-brownsub hover:scale-105 hover:drop-shadow-xl md:ml-4 md:mt-0 hover:-rotate-2"
          to="https://play.google.com/store/apps/details?id=com.sekky.kibunya&hl=en_US"
          target="_blank"
          >Androidダウンロード</NuxtLink
        >
      </div>
    </div>

    <div id="feather" class="mb-40">
      <ul class="grid grid-cols-1 gap-3 md:grid-cols-3">
        <li
          class="flex flex-col items-center p-6 bg-white rounded-lg shadow-lg"
        >
          <p class="mb-2 font-bold">特徴1</p>
          <div>めちゃ可愛い</div>
        </li>
        <li
          class="flex flex-col items-center p-6 bg-white rounded-lg shadow-lg"
        >
          <p class="mb-2 font-bold">特徴2</p>
          <div>めちゃ可愛い</div>
        </li>
        <li
          class="flex flex-col items-center p-6 bg-white rounded-lg shadow-lg"
        >
          <p class="mb-2 font-bold">特徴3</p>
          <div>
            めちゃ可愛いめちゃ可愛いめちゃ可愛いめちゃ可愛いめちゃ可愛いめちゃ可愛い
          </div>
        </li>
      </ul>
    </div>

    <News />
  </div>
</template>
