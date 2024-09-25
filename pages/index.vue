<template>
  <main class="pt-5">
    <div>
      <Logo class="nav-logo w-[100px] m-auto" />
    </div>
    <div class="slogan text-center">
      <h3>We build a better world.</h3>
      <h3>Chúng tôi xây dựng một thế giới tốt-đẹp-hơn.</h3>
    </div>
    <nav class="w-fit m-auto mt-3 p-3">
      <ul class="flex gap-1">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/">Management</NuxtLink></li>
        <li><NuxtLink to="/">IoT</NuxtLink></li>
        <li><NuxtLink to="/">AI</NuxtLink></li>
        <li><NuxtLink to="/">TRC Living</NuxtLink></li>
      </ul>
    </nav>

    <div>
      <NuxtPage />
    </div>
  </main>
</template>
<style>
li:hover {
  font-weight: bold;
}

ul li {
  @apply bg-gray-200 p-3 cursor-pointer;
}
</style>
