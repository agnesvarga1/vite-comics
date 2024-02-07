<script>
export default {
  name: "AppHeader",
  data() {
    return {
      arrayNavMenu: [
        {
          linkName: "characters",
          link: "#",
          current: false,
        },
        {
          linkName: "comics",
          link: "#",
          current: true,
        },
        {
          linkName: "movies",
          link: "#",
          current: false,
        },
        {
          linkName: "tv",
          link: "#",
          current: false,
        },
        {
          linkName: "games",
          link: "#",
          current: false,
        },
        {
          linkName: "collectibles",
          link: "#",
          current: false,
        },
        {
          linkName: "videos",
          link: "#",
          current: false,
        },
        {
          linkName: "fans",
          link: "#",
          current: false,
        },
        {
          linkName: "news",
          link: "#",
          current: false,
        },
        {
          linkName: "shop",
          link: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <nav>
      <figure>
        <img src="../assets/img/dc-logo.png" alt="logo" width="90" />
      </figure>
      <ul>
        <li
          :class="item.current ? `active` : ``"
          v-for="(item, index) in arrayNavMenu"
          :key="index"
        >
          <a :href="item.link">{{ item.linkName }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
header {
  background-color: #fff;
  nav {
    width: 70%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 1.5rem;
    figure {
      padding-block: 10px;
    }
    ul {
      height: 110px;
      display: flex;
      align-items: center;
      gap: 1rem;

      li {
        height: inherit;
        a {
          display: flex;
          align-items: center;
          height: inherit;
          color: #303030;
          text-transform: uppercase;
          font-weight: bold;
        }
      }
    }
  }
}
</style>
