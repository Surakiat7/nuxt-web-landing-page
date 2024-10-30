<script setup lang="ts">
useHead({
  title: 'OWNDAYS Labs',
  meta: [
    { name: 'description', content: 'Podux Podcast landing page website.' },
  ],
  link: [
    { rel: 'icon', type: 'image/png', href: '/logo-owndays-labs.png' }
  ],
})
</script>
<template>
    <div>
        <SectionsHomeHeroSection/>
        <SectionsHomeLatestCollection />
        <SectionsHomePopularSunglasses />
        <SectionsAboutUs />
        <SectionsWhyUs/>
        <SectionsCallToAction/>
    </div>
</template>