<template>
  <nav>
    <NuxtLink to="/products" class="hover:text-blue-200" >Product Catalog</NuxtLink>
    <NuxtLink to="/contact" class="hover:text-blue-200">Field Service</NuxtLink>
    <NuxtLink to="/about-us" class="hover:text-blue-200">About Us</NuxtLink>
    <NuxtLink to="/contact" class="hover:text-blue-200">{{ $t('messages.general.contact') }}</NuxtLink>
    <NuxtLink to="/contact" class="hover:text-blue-200">{{ $t('Account Login') }}</NuxtLink>
  </nav>
</template>
