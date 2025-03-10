<script setup></script>
<template>
  <nav class="navbar bg-white shadow-md shadow-gray-500 has-outline">
    <div class="navbar-brand items-center sm:items-stretch sm:justify-center">
      <div class="flex shrink-0 items-center">Logic Lab</div>
    </div>
    <!-- Mobile menu -->
    <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
      <button
        type="button"
        @click="toggleMenu"
        class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-700 hover:bg-blue-950 hover:text-blue-950 focus:ring-2 focus:ring-white focus:outline-hidden focus:ring-inset"
        aria-controls="mobile-menu"
        aria-expanded="false"
      >
        <span class="absolute -inset-0.5"></span>
        <span class="sr-only">Open main menu</span>

        <svg
          v-if="!isMobileMenuOpen"
          class="block size-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          aria-hidden="true"
          data-slot="icon"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
          />
        </svg>

        <svg
          v-else
          class="hidden size-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          aria-hidden="true"
          data-slot="icon"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6 18 18 6M6 6l12 12"
          />
        </svg>
      </button>
    </div>
    <!-- Mobile menu -->
  </nav>
</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
