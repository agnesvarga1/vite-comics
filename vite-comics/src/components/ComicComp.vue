<script>
export default {
  props: {
    img: String,
    title: String,
  },
};
</script>
<template>
  <div class="comic">
    <img :src="img" alt="book cover" />
    <h4>{{ title }}</h4>
  </div>
</template>

<style lang="scss" scoped>
.comic {
  margin-bottom: 1rem;
  flex-basis: calc(100% / 6 - 20px);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  img {
    width: 200px;
    aspect-ratio: 1;
  }
  h4 {
    padding-block: 0.4rem;
    text-align: center;
    font-weight: 100;
  }
}
</style>
