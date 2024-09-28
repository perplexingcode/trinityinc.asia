<template>
  <main class="pt-5">
    <div>
      <Logo class="nav-logo w-[100px] m-auto" />
    </div>
    <div class="slogan text-center font-[500]">
      <h3>We build a better world.</h3>
      <h3>Chúng tôi xây dựng một thế giới tốt-đẹp-hơn.</h3>
    </div>
    <nav class="w-fit m-auto mt-3 p-3">
      <ul class="flex gap-1">
        <li class="active">
          <NuxtLink to="/"
            ><div class="flex flex-col items-center">
              <span>Management</span
              ><span class="text-xs text-gray-700">Phase III</span>
            </div></NuxtLink
          >
        </li>
        <li>
          <NuxtLink to="/"
            ><div class="flex flex-col items-center">
              <span>AI</span><span class="text-xs text-gray-700">Phase IV</span>
            </div></NuxtLink
          >
        </li>
        <li>
          <NuxtLink to="/"
            ><div class="flex flex-col items-center">
              <span>IoT</span><span class="text-xs text-gray-700">Phase V</span>
            </div></NuxtLink
          >
        </li>
        <li>
          <NuxtLink to="/"
            ><div class="flex flex-col items-center">
              <span>Trinity Life</span
              ><span class="text-xs text-gray-700">D3</span>
            </div></NuxtLink
          >
        </li>
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
ul li.active {
  @apply bg-yellow-300 p-3 cursor-pointer;
}
</style>
