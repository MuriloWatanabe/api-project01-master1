<script>
export default {
  props: ["serie"],
  methods: {
    getImageUrl(poster_path) {
      return `https://image.tmdb.org/t/p/w500${poster_path}`;
    },
  },
};
</script>

<template>
  <ul>
    <li>
      <a href="#">
        <img :src="getImageUrl(serie.poster_path)" />
      </a>
      <span>{{ serie.name }}</span>
    </li>
  </ul>
</template>
<style scoped>
@import "@/assets/base.css";

img {
  width: 180px;
  border-radius: 20px;
  margin-bottom: 2rem;
}
</style>
