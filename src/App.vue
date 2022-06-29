<script setup lang="ts">
import { RouterView } from "vue-router";
</script>

<template>
  <header>
    <img src="./assets/spy.png" alt="" />
    <h1>Spiontyggis.no</h1>

    <router-link class="router-link-game" to="game">Prøv spillet</router-link>
  </header>

  <RouterView />
</template>

<style>
@import "@/assets/base.css";

header {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;

  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

header h1 {
  font-family: "Special Elite", cursive;
  color: black;
  font-size: 2rem;
}

img {
  height: 4rem;
}

.router-link-game {
  border: solid black;
  background-color: var(--color-background);
  color: var(--color-text);
  font-size: 2rem;
  text-decoration: none;

  margin-left: auto;
  padding: 0 0.5rem 0 0.5rem;
}
</style>
