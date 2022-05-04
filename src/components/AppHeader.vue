<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="logo">
        <nav>
          <ul>
            <li v-for="(item, index) in links" :key="index">{{item.testo}}</li>
          </ul>
        </nav>
    </header>
</template>

<script>
export default {
  name: 'AppHeader',
  data(){
        return {
            links: [
                {
                    testo: "Characters",
                    link: "",
                    active: false,
                },
                {
                    testo: "Comics",
                    link: "",
                    active: true,
                },
                {
                    testo: "Movies",
                    link: "",
                    active: false,
                },
                {
                    testo: "Tv",
                    link: "",
                    active: false,
                },
                                {
                    testo: "Games",
                    link: "",
                    active: false,
                },
                {
                    testo: "Collectibles",
                    link: "",
                    active: true,
                },
                {
                    testo: "VIdeos",
                    link: "",
                    active: false,
                },
                {
                    testo: "Fans",
                    link: "",
                    active: false,
                },
                                {
                    testo: "News",
                    link: "",
                    active: false,
                },
                {
                    testo: "Shop",
                    link: "",
                    active: false,
                }
            ]
        }
    }
}
</script>

<style lang="scss">
  @import "../style/variables.scss";

  header {
    @include my-container;
    display: flex;
    justify-content: space-between;
    padding: 1em 0;
    
    img {
      width: 70px;
    }

    nav ul {
      height: 100%;
      list-style-type: none;
      display: flex;
      align-items: center;

      li {
        font-size: 12px;
        text-transform: uppercase;
        padding: 0 1em;
      }
    }
  }

  .active {
    border-bottom: 3px solid $bg-blue;
    color: $bg-blue;
  }
</style>