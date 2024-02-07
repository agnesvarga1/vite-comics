<script>
export default {
  name: "Cards",
  data() {
    return {
      arrayCards: [
        {
          path: "../../src/assets/img/buy-comics-digital-comics.png",
          title: "Digital Comics",
        },
        {
          path: "../../src/assets/img/buy-comics-merchandise.png",
          title: "DC merchandise",
        },
        {
          path: "../../src/assets/img/buy-comics-subscriptions.png",
          title: "Subscription",
        },
        {
          path: "../../src/assets/img/buy-comics-shop-locator.png",
          title: "comic shop locator",
        },
        {
          path: "../../src/assets/img/buy-dc-power-visa.svg",
          title: "DC power visa",
        },
      ],
    };
  },
};
</script>

<template>
  <div>
    <div class="card-container">
      <div v-for="(item, index) in arrayCards" :key="index" class="card">
        <figure>
          <img width="60" :src="item.path" alt="icon-services" />
        </figure>
        <h3>{{ item.title }}</h3>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
div {
  background-color: #0282f9;
  .card-container {
    padding: 3rem 5rem;
    width: 75%;
    margin: 0 auto;
    display: flex;
    gap: 20px;
    .card {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      gap: 15px;
    }
  }
}
</style>
