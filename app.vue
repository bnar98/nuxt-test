<template>
  <div>
    <a
      :href="`https://www.facebook.com/sharer/sharer.php?u=${url}text=${title}`"
      target="_blank"
    >
      SHAREE
    </a>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
  </div>
</template>
<script setup lang="ts">
useHead({
  title: "My App",
  meta: [
    { name: "og:image", content: "https://www.tiwarnews.net/logo.png" },
    {
      name: "og:description",
      content:
        ".... social-links is a set of social media share links working with React and Svelte",
    },
    { name: "og:title", content: "...My amazing FHFDH site. bnarrr" },
  ],
});
const url = "https://nuxt-test-lovat-three.vercel.app/";
const title = "hh";
</script>
