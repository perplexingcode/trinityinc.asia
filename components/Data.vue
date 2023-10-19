<template>
  <div>
    <slot></slot>
  </div>
</template>
<script setup>
const state = reactive({});
const events = reactive({});
const config = reactive({});

provide('state', state);
provide('events', events);
provide('config', config);
</script>
<style></style>
