<template>
  <div class="grid grid-flow-col justify-center content-center py-8 gap-10">
    <div v-for="lib in libraries" :key="lib.name">
      <a :href="lib.link" :title="lib.name" target="_blank" rel="noopener">
        <img :src="lib.logoLight" loading="lazy" class="dark:hidden w-24 h-24" />
        <img :src="lib.logoDark" loading="lazy" class="hidden dark:block w-24 h-24" />
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">
const libraries = [
  {
    name: 'PrimeVue',
    link: 'https://primevue.org/inputtext/#veevalidate',
    logoLight: 'https://primefaces.org/cdn/primevue/images/logo.svg',
    logoDark: 'https://primefaces.org/cdn/primevue/images/logo.svg',
  },
  {
    name: 'Vuetify',
    link: 'https://vuetifyjs.com/en/components/forms/#vee-validate',
    logoLight: 'https://cdn.vuetifyjs.com/docs/images/logos/vuetify-logo-v3-light.svg',
    logoDark: 'https://cdn.vuetifyjs.com/docs/images/logos/vuetify-logo-v3-light.svg',
  },
];
</script>
