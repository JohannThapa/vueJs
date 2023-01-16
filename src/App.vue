<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="navbar">
    <div class="wrapper">
      <nav>
        <img
          alt="Vue logo"
          class="logo"
          src="@/assets/logo.svg"
          width="50"
          height="50"
        />
        <RouterLink class="fg-1" to="/">Home</RouterLink>
        <RouterLink class="fg-1" to="/about">About</RouterLink>
        <RouterLink class="fg-1" to="/landing">Landing</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
