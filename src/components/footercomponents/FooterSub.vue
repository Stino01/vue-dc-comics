<template>
    <div class="bg">
        <nav>
            <ul>
                <li v-for="(items, index) in buyOption" :key="index">
                    <img :src="items.img" :alt="items.testo">
                    <p>{{items.testo}}</p>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
  name: 'FooterSub',
   data(){
        return {
            buyOption: [
                {
                    testo: "Digital Comics",
                    link: "",
                    img: require("../../assets/img/buy-comics-digital-comics.png"),
                },
                {
                    testo: "Dc Merchandise",
                    link: "",
                    img: require("../../assets/img/buy-comics-merchandise.png"),
                },
                {
                    testo: "Subscription",
                    link: "",
                    img: require("../../assets/img/buy-comics-subscriptions.png"),
                },
                {
                    testo: "Comic Shop Locator",
                    link: "",
                    img: require("../../assets/img/buy-comics-shop-locator.png"),
                },
                                {
                    testo: "Dc Power Visa",
                    link: "",
                    img: require("../../assets/img/buy-dc-power-visa.svg"),
                },
            ]
        }
    }
}
</script>

<style lang="scss">
  @import "../../style/variables.scss";

  .bg {
      background-color: $bg-blue;

      nav {
          @include my-container;

          ul {
              list-style-type: none;
              @include my-flex;
              justify-content: center;
              align-items: center;
              padding: 2em 0;

              li {
                text-transform: uppercase;
                @include my-flex;
                justify-content: center;
                align-items: center;
                padding: 0 1em;

                img {
                    width: 3em;
                }

                p {
                    font-size: 14px;
                    color: white;
                    padding: 10px;
                }

                &:nth-child(4) img {
                    width: 2em;
                }
              }
          }
      }
  }
</style>