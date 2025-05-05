<template>
  <section
    class="container mx-auto px-4 py-4 grid grid-cols-1 md:grid-cols-3 gap-6"
  >
    <!-- Left: Main Featured News -->
    <div
      class="relative h-[300px] md:h-[615px] col-span-1 md:col-span-2 rounded overflow-hidden"
    >
      <img
        src="/images/campus.jpg"
        alt="Main Feature"
        class="absolute inset-0 w-full h-full object-cover object-bottom"
      />
      <div class="absolute inset-0 bg-black bg-opacity-50"></div>

      <div
        class="relative z-10 h-full flex flex-col justify-end p-4 md:p-6 text-white"
      >
        <span class="bg-[#F4796C] px-2 py-1 text-xs rounded w-fit mb-2">
          ভর্তি তথ্য
        </span>
        <h2 class="text-lg md:text-xl font-bold mb-2 md:mb-3 leading-snug">
          ২০২৫ সালের পাবলিক বিশ্ববিদ্যালয় ভর্তি নির্দেশিকা ও ইউনিটভিত্তিক
          প্রস্তুতি গাইড
        </h2>
        <div
          class="flex flex-wrap items-center text-xs md:text-sm space-x-2 md:space-x-4 opacity-90"
        >
          <span>🖊️ By Admin</span>
          <span>📅 27 August, 2024</span>
          <span>⏱️ 20 Mins</span>
        </div>
      </div>
    </div>

  
    <div class="h-[300px] md:h-[615px] col-span-1 md:col-span-1 flex flex-col justify-between space-y-4">
      <div
        v-for="(item, index) in newsList"
        :key="index"
        class="relative h-[150px] md:h-[192px] lg:h-[320px] rounded overflow-hidden"
      >
        <img
          :src="item.image"
          alt="News"
          class="absolute inset-0 w-full h-full object-cover object-bottom"
        />
        <div class="absolute inset-0 bg-black bg-opacity-50"></div>

        <!-- Align to bottom -->
        <div
          class="relative z-10 h-full flex flex-col justify-end p-2 md:p-3 text-white"
        >
          <span class="bg-[#F4796C] px-2 py-0.5 text-xs rounded w-fit mb-1"
            >ভর্তি তথ্য</span
          >
          <p class="text-xs md:text-sm font-semibold leading-5">
            {{ item.title }}
          </p>
          <span class="text-xs mt-1">{{ item.date }}</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const newsList = [
  {
    title: "স্কুল, কলেজ ও বিশ্ববিদ্যালয়ের একাডেমিক ক্যালেন্ডার ও পরীক্ষার সময়সূচি (২০২৫)",
    date: "27 August, 2024",
    image: "/images/img1.jpg",
  },
  {
    title: "পাঠ্যপুস্তক থেকে রুটিন পর্যন্ত: একাডেমিক জীবনের নির্দেশনা",
    date: "27 August, 2024",
    image: "/images/img2.jpg",
  },
  {
    title: "একাডেমিক রেজাল্ট চেক করার সহজ উপায়",
    date: "27 August, 2024",
    image: "/images/img3.jpg",
  },
];
</script>
