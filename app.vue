<template>
  <div>
    <Data>
      <NuxtPage />
    </Data>
  </div>
</template>
<script setup>
// Add favicon and title
useHead({
  title: 'Trinity Inc - We build a better world',
  link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.svg' }],
});
</script>
