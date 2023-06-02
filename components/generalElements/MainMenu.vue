<template>
  <nav>
    <NuxtLink to="/">{{ $t('messages.general.home') }}</NuxtLink>
    <NuxtLink to="/products">Product Catalog</NuxtLink>
    <NuxtLink to="/categories">{{ $t('messages.shop.category', 2) }}</NuxtLink>
    <NuxtLink to="/contact">About Us</NuxtLink>
    <NuxtLink to="/contact">{{ $t('messages.general.contact') }}</NuxtLink>
    <NuxtLink to="/contact">{{ $t('Account Login') }}</NuxtLink>
  </nav>
</template>
