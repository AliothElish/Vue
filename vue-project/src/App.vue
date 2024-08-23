<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <TheWelcome />
    <iframe
      src="https://chat.cpii.ai/embed?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjY5NDk0M2U5MzYzOWFiMzNkZjA4M2Y5IiwicHJvamVjdF9pZCI6IjY2OTVjZWZhOTM2MzlhYjMzZGYwOGRiOCIsImV4cCI6MTcyNDkyNzI3OX0.0yZPRHjF8PKk0Zp_K8_uj20TOcc4P5qkNVdWvxLHxEc&name=CPII ChatBot" width="100%">
    </iframe>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
