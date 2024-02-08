<script>
export default {
  name: "Cards",
  data() {
    return {
      arrayCards: [
        {
          path: "buy-comics-digital-comics.png",
          title: "Digital Comics",
        },
        {
          path: "buy-comics-merchandise.png",
          title: "DC merchandise",
        },
        {
          path: "buy-comics-subscriptions.png",
          title: "Subscription",
        },
        {
          path: "buy-comics-shop-locator.png",
          title: "comic shop locator",
        },
        {
          path: "buy-dc-power-visa.svg",
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
          <img
            width="50"
            :src="`../../src/assets/img/${item.path}`"
            alt="icon-services"
          />
        </figure>
        <h4>{{ item.title }}</h4>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
div {
  background-color: $blue-main;

  .card-container {
    padding: 2rem 5rem;
    width: 75%;
    margin: 0 auto;
    display: flex;
    gap: 20px;
    .card {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      gap: 15px;
      figure {
        img {
          height: 60px;
        }
      }
      h4 {
        text-transform: uppercase;
        font-weight: 100;
      }
    }
  }
}
</style>
