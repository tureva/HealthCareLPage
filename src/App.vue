<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <section class="h-screen">
    <header class="h-14 flex items-center justify-center bg-black sticky top-0">
      <nav class="flex items-center justify-between">
        <div class="flex items-center mr-96">
          <img src="./assets/logo.svg" alt="logo" class="w-8 h-12" />
          <p class="text-white">ue Mastery</p>
        </div>
        <div class="flex ml-96">
          <ul class="flex text-white">
            <li class="mr-10 text-lg p-2"><RouterLink to="/">Home</RouterLink></li>
            <li class="mr-10 text-lg p-2"><RouterLink to="/about">About</RouterLink></li>
            <li class="mr-10 text-lg p-2"><RouterLink to="/contact">Contacts</RouterLink></li>
            <li class="mr-10 text-lg p-2"><RouterLink to="#">Gallery</RouterLink></li>
          </ul>
        </div>
      </nav>
    </header>
    <main>
      <RouterView />
    </main>
  </section>
  
</template>
