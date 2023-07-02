<template>
  <main class="pt-5">
  <div>
    <img class="nav-logo w-[100px] m-auto" src="~/assets/img/logo-concept.svg" />
  </div>
  <nav class="w-fit m-auto mt-3 bg-gray-200 p-3">
    <ul class="flex gap-3">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/test">Management</NuxtLink></li>
        <li><NuxtLink to="/today">IoT</NuxtLink></li>
        <li><NuxtLink to="/category">AI</NuxtLink></li>
        </ul>
  </nav>
  <div>
    <NuxtPage />
  </div>
</main>
</template>
<style  >
li:hover {
  font-weight: bold;
}
</style>
