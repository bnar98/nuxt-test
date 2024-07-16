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
    {
      name: "og:image",
      content:
        "https://d38b044pevnwc9.cloudfront.net/cutout-nuxt/enhancer/2.jpg",
    },
    {
      name: "og:description",
      content:
        ".... social-links is a set of social media share links working with React and Svelte",
    },
    { name: "og:title", content: "...My amazing FHFDH site. bnarrr gyannn" },
  ],
});
const url = "https://nuxt-test-lovat-three.vercel.app/";
const title = "hh";
</script>
