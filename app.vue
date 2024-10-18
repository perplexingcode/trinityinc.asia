<template>
  <div>
    <Data>
      <NuxtPage />
    </Data>
  </div>
</template>
<script setup>
const trinityAI = {
  src: 'https://mindmaid.ai/embed-assistant.js',
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
  link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon-plain.svg' }],
  script: [trinityAI],
});
</script>
<style>
.box-chat-embed svg {
  stroke: #003eb3;
}

.box-chat-embed img:last-child {
  padding: 6px !important;
  border-radius: 40% !important;
  filter: drop-shadow(rgba(0, 0, 0, 0.1) 0px 0px 2px) !important;
}

.greetingBox {
  background: #fefefa !important;
  filter: drop-shadow(rgba(0, 0, 0, 0.1) 0px 0px 6px) !important;
}

.greetingBox circle {
  fill: #f8fafc !important;
  stroke: none;
}

.greetingBox p {
  color: #051c2c !important;
  font-family: Be Vietnam Pro, sans-serif !important;
  font-weight: 500 !important;
  text-align: center !important;
  padding-left: 0.5rem !important;
  padding-right: 0.55rem !important;
}

.greetingBox img {
  display: none;
}
</style>
