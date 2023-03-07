<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/portfolio" class="font-bold"
          >Mia Codes Portfolio</NuxtLink
        >
      </nav>
    </header>
    <!-- page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
    <footer class="container mx-auto p-4 flex justify-between border-t-2">
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/splash">A Tech Splash</NuxtLink></li>
        <li><NuxtLink to="/portfolio">Portfolio</NuxtLink></li>
        <li><NuxtLink to="/about">About Me</NuxtLink></li>
        <li><NuxtLink to="/contact">Contact Me</NuxtLink></li>
        <li><NuxtLink to="/estimate">Estimate</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: #12b488;
}
</style>
