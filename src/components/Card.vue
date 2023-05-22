<script>
export default {
  props: {
    cardData: Object,
  },
};
</script>
<template>
  <div class="card">
    <img :src="cardData.card_images.image_url_small" :alt="cardData.name" />
    <h2>{{ cardData.name }}</h2>
    <div class="type">{{ cardData.archetype }}</div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc((100% - 4rem) / 6);
}
</style>
