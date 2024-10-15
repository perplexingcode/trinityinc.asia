<template>
  <div>
    <Data>
      <NuxtPage />
    </Data>
  </div>
</template>
<script setup>
const trinityAI = {
  src: 'https://mindmaid.ai/embed-assistant.js" data-chat-service="Salebot" data-bot-id="bd409e68-7395-49d2-9fd1-36b6bee222d7',
  'data-chat-service': 'Salebot',
  'data-bot-id': 'bd409e68-7395-49d2-9fd1-36b6bee222d7',
  'data-chat-width': '450px',
  'data-chat-height': '600px',
  'data-bubble-color': '',
  async: true,
  defer: true,
};
useHead({
  title: 'Trinity Inc - We build a better world',
  link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.svg' }],
  script: [trinityAI],
});
</script>
