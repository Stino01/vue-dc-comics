<template>
    <div class="bg-hero"> 
        <div class="container">
          <div>
            <h2>DC Comics</h2>
            <ul>
              <li v-for="(items, index) in data1" :key="index">{{items.testo}}</li>
            </ul>
            <h2>Shop</h2>
            <ul>
              <li v-for="(items, index) in data2" :key="index">{{items.testo}}</li>
            </ul>
          </div>
          <div>
            <h2>DC</h2>
            <ul>
              <li v-for="(items, index) in data3" :key="index">{{items.testo}}</li>
            </ul>
          </div>
          <div>
            <h2>Sites</h2>
            <ul>
              <li v-for="(items, index) in data4" :key="index">{{items.testo}}</li>
            </ul>
          </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'FooterInfo',
  data(){
        return {
            data1: [
                {
                    testo: "Characters",
                    link: "",
                },
                {
                    testo: "Comics",
                    link: "",
                },
                {
                    testo: "Movies",
                    link: "",
                },
                {
                    testo: "TV",
                    link: "",
                },
                {
                    testo: "Games",
                    link: "",
                },
                {
                    testo: "Videos",
                    link: "",
                },
                {
                    testo: "News",
                    link: "",
                },
            ],
            data2: [
                {
                    testo: "Shop DC",
                    link: "",
                },
                {
                    testo: "Shop DC Collectibles",
                    link: "",
                },
            ],
            data3: [
                {
                    testo: "Term Of Use",
                    link: "",
                },
                {
                    testo: "Privacy policy",
                    link: "",
                },
                {
                    testo: "Ad Choices",
                    link: "",
                },
                {
                    testo: "Advertising",
                    link: "",
                },
                {
                    testo: "Jobs",
                    link: "",
                },
                {
                    testo: "Subscriptions",
                    link: "",
                },
                {
                    testo: "Talent Workshops",
                    link: "",
                },
                {
                    testo: "CPSC Certificates",
                    link: "",
                },
                {
                    testo: "Ratings",
                    link: "",
                },
                {
                    testo: "Shop Help",
                    link: "",
                },
                {
                    testo: "Contact Us",
                    link: "",
                },
            ],
            data4: [
                {
                    testo: "DC",
                    link: "",
                },
                {
                    testo: "MAD Magazine",
                    link: "",
                },
                {
                    testo: "DC Kids",
                    link: "",
                },
                {
                    testo: "DC Universe",
                    link: "",
                },
                {
                    testo: "DC Power Visa",
                    link: "",
                },
            ],
        }
    }
}
</script>

<style lang="scss">
  @import "../../style/variables.scss";

  .bg-hero {
    background-image: url(../../assets/img/footer-bg.jpg);
    padding: 2em 0;

    .container {
      @include my-container;
      @include my-flex;

      div {
        display: flex;
        flex-flow: column nowrap;
        padding: 0 1em;

        h2 {
          padding: 0.8em 0;
          color: white;
          text-transform: uppercase;
          font-size: 18px;
        }

        ul {
          list-style-type: none;

          li {
            padding: 2px 0;
            color: #70766F;
          }
        }
      }
    }
  }
</style>