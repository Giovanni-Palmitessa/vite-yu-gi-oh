<script>
export default {
  props: {
    cardData: Object,
  },
};
</script>
<template>
  <div class="card">
    <img :src="cardData.image" :alt="cardData.name" />
    <h2>{{ cardData.name }}</h2>
    <div class="type">{{ cardData.type }}</div>
  </div>
</template>

<style lang="scss" scoped></style>
