<template>
  <header class=" bg-[#192551] shadow-sm top-0 shadow-light-500 z-40 sticky">
    <div class="container flex py-4 items-center justify-between">
      <div class="flex items-center">
        <MenuTrigger class="md:hidden" />
        <Logo class="md:w-[160px]" />
      </div>
      <MainMenu class="text-base font-bold text-white pt-8 gap-24 items-center hidden md:flex lg:px-4 "  />
      <div class="flex gap-4 justify-end items-center md:w-[160px]">
        <CartTrigger class="text-white hover:text-blue-200 pt-7 font-bold" />
      </div>
    </div>
  </header>
  <div class=" bg-primary-light">
    <p class=" text-right font-semibold text-white pr-6">Call us today:  <a class="font-bold text-blue-200" href=”callto://+17085340008″>+1 (708) 534-0008</a>

|  <a class="font-bold text-blue-200" href=”callto://+1882846267″>+1(888) 284-6267</a>
</p>
  </div>
</template>
