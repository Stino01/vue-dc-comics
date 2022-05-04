<template>
    <div class="bgsing">
        <div class="container"> 
          <div class="button"><span>Sing-up now!</span></div>
          <div>
            <p>Follow us</p>
            <ul>
              <li v-for="(items, index) in social" :key="index"><img :src="items.img" :alt="items.testo"></li>
            </ul>
          </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'FooterSing',
  data(){
        return {
            social: [
                {
                    testo: "Facebook",
                    link: "",
                    img: require("../../assets/img/footer-facebook.png"),
                },
                {
                    testo: "Twitter",
                    link: "",
                    img: require("../../assets/img/footer-twitter.png"),
                },
                {
                    testo: "Youtube",
                    link: "",
                    img: require("../../assets/img/footer-youtube.png"),
                },
                {
                    testo: "Pintest",
                    link: "",
                    img: require("../../assets/img/footer-pinterest.png"),
                },
                                {
                    testo: "Periscope",
                    link: "",
                    img: require("../../assets/img/footer-periscope.png"),
                },
            ]
        }
    }
}
</script>

<style lang="scss">
  @import "../../style/variables.scss";

  .bgsing {
    background-color: $bg-grey;

    .container {
      @include my-container;
      @include my-flex;
      justify-content: space-between;
      align-items: center;
      padding: 2em 0;

      .button {
        border: 1px solid $bg-blue;

        span {
          color: white;
          text-transform: uppercase;
          padding: 10px
        }
      }

      div {
        @include my-flex;
        align-items: center;

        p {
          font-size: 18px;
          text-transform: uppercase;
          color: $bg-blue;
          font-weight: 900;
          padding-right: 1em
        }

        ul {
          @include my-flex;
          list-style-type: none;

          li {
            margin: 0 0.5em;
          }
        }
      }
    }
  }
</style>