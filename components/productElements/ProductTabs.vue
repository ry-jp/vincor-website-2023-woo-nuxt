<script setup>
const props = defineProps({
  product: { type: Object, default: null },
});

const show = ref(0);
</script>

<template>
  <div>
    <nav class="border-b flex gap-8 tabs">
      <a :class="show === 0 ? 'active' : ''" @click.prevent="show = 0">{{ $t('messages.shop.productDescription') }}</a>
      <a :class="show === 1 ? 'active' : ''" @click.prevent="show = 1">Document</a>
    </nav>
    <div class="tab-contents">
      <div v-if="show === 0" class="font-light mt-8 prose" v-html="product.description"></div>
      <div v-if="show === 1">
        <div class="flex flex-wrap gap-32 items-start">
          <div class="flex max-w-sm gap-4 prose">
          </div>
          <div class="divide-y flex-1">
            <p class="text-red-600 text-lg">{{ product.category }}</p>
            <p class="text-red-600 text-lg">{{ product.sku }}</p>
<div>
<iframe :src="`/pdf/${product.sku}.pdf`" width="100%" height="1024">
  </iframe>

</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="postcss">
.tabs a {
  @apply border-transparent border-b-2 text-lg pb-8;
  margin-bottom: -1px;
}

.tabs a.active {
  @apply border-primary text-primary;
}
</style>
