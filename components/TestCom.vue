<template>
  <div>
    <PopoverButton
      class="inline-flex items-center justify-center rounded-xl p-2 text-[#426058] bg-gray-100 hover:bg-gray-200 focus:outline-none"
    >
      <span class="sr-only">Open menu</span>
      <Icon name="zondicons:menu" class="h-5 w-5 md:h-8 md:w-8"></Icon>
    </PopoverButton>
  </div>
</template>

<script setup>

import {
  Popover,
  PopoverButton,
  PopoverGroup,
  PopoverPanel,
} from "@headlessui/vue";
</script>
