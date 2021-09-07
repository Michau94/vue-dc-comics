<template>
  <header>
    <div class="container wrapper">
      <img src="../assets/img/dc-logo.png" alt="Logo" />

      <nav>
        <ul>
          <li
            :class="{ active: link.current }"
            v-for="(link, index) in header"
            :key="index"
            @click="currentLink(index)"
          >
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      header: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
  methods: {
    currentLink(idx) {
      this.header.forEach((el, ind) => {
        ind == idx ? (el.current = true) : (el.current = false);
      });
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";

header {
  height: 200px;
}

.wrapper {
  align-items: center;
}

nav ul {
  display: flex;
  align-items: center;
  height: 200px;

  li {
    margin: 10px;
    list-style-type: none;
    height: 100%;
    line-height: 200px;

    &:hover,
    &.active {
      border-bottom: 5px solid;
      border-color: $base-color;
    }
    a {
      text-decoration: none;
      text-transform: uppercase;
      font-weight: bold;
      color: $text-secondary;
      font-size: 0.8rem;
      padding: 10px;
    }
  }
}
</style>
