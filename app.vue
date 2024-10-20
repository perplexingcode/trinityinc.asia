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

const htmlMessages = [
  `Hello! I'm Trinity. How can I help you today?`,
  `Did you know that blue is the only color not naturally found in nature?
  This makes it a symbol of novelty.`,
  `Speed is the most important thing in business.`,
  `A kind heart remains calm amidst the storm. A strong mind sees through its dark clouds.`,
  `Existence is the highest virtue.`,
  `Play reasonably, opportunity will come.`,
  `Precision is the foundation of honesty.`,
  `Abstraction is elevation.`,
  // `Mistakes and successes converge at the knot of one's destiny.`,
];
onMounted(async () => {
  await nextTick();
  if (!process.client) return;
  const aiText = document.querySelector('.greetingBox p');
  setInterval(() => {
    aiText.textContent =
      htmlMessages[Math.floor(Math.random() * htmlMessages.length)];
  }, 13000);
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
  max-width: 33rem;
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
  padding-right: 0.5rem !important;
  white-space: pre-wrap !important;
}

.greetingBox p + img {
  display: none;
}
</style>
