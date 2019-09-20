<template>
  <div class="home">
    <section class="hero">
      <v-container>
        <v-row no-gutters>
          <v-col md="4" class="bg-symbol-1 mt-12">
            <h4
              v-scroll-reveal.reset="revealFromBottom"
              class="overline mb-4 mb-5"
            >
              Premium Coffee
            </h4>
            <h1
              v-scroll-reveal.reset="revealFromBottom"
              class="display-1 font-weight-medium"
            >
              A cup of coffee is one of the most important simple pleasures in
              life
            </h1>
            <v-btn
              v-scroll-reveal="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-10 py-4 mt-10"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> Shop now
            </v-btn>
          </v-col>
          <v-col id="hero__image-wrap" md="8">
            <v-img
              v-scroll-reveal.reset="revealFromRight"
              class="hero__image"
              contain
              :src="require('~/assets/images/Spilled-Coffee-Beans.png')"
              :lazy-src="require('~/assets/images/Spilled-Coffee-Beans.png')"
            ></v-img>
          </v-col>
        </v-row>
      </v-container>
      <div v-scroll-reveal.reset="revealFromRight" class="hero__dots"></div>
    </section>

    <section class="py-12 mt-12">
      <v-container>
        <div class="d-flex justify-center">
          <div
            v-scroll-reveal.reset="revealFromRightWithDelay(100)"
            class="icon-box"
          >
            <div class="icon-box__icon mb-7">
              <v-icon x-large>mdi-leaf</v-icon>
            </div>
            <h4 class="title">Quality coffee cultivated by Good</h4>
          </div>
          <div
            v-scroll-reveal.reset="revealFromRightWithDelay(200)"
            class="icon-box"
          >
            <div class="icon-box__icon mb-7">
              <v-icon x-large>mdi-flower-tulip-outline</v-icon>
            </div>
            <h4 class="title">Flavour Single Origin Froth in spoon iced</h4>
          </div>
          <div
            v-scroll-reveal.reset="revealFromRightWithDelay(300)"
            class="icon-box"
          >
            <div class="icon-box__icon mb-7">
              <v-icon x-large>mdi-sprout-outline</v-icon>
            </div>
            <h4 class="title">Milk grounds chicory beans single origin</h4>
          </div>
          <div
            v-scroll-reveal.reset="revealFromRightWithDelay(400)"
            class="icon-box"
          >
            <div class="icon-box__icon mb-7">
              <v-icon x-large>mdi-flower-outline</v-icon>
            </div>
            <h4 class="title">Coffee irish robusta spoon robust.</h4>
          </div>
        </div>
      </v-container>
    </section>

    <section class="py-12">
      <v-container>
        <v-row align="center" no-gutters>
          <v-col lg="6">
            <div
              v-scroll-reveal.reset="revealPointedImg1"
              class="pointed-img-wrap"
            >
              <v-img
                :src="require('~/assets/images/coffee-cups.jpg')"
                class="pointed-img left"
              ></v-img>
            </div>
          </v-col>
          <v-col lg="6" class="bg-symbol-2">
            <h4 v-scroll-reveal.reset="revealFromBottom" class="overline mb-4">
              Premium Coffee
            </h4>
            <h5 v-scroll-reveal.reset="revealFromBottom" class="display-2">
              Quality coffee <br />
              cultivated by Good
            </h5>
            <p
              v-scroll-reveal.reset="revealFromBottom"
              class="title font-weight-regular py-5 pr-10"
            >
              Our love for specialty coffee is never-ending. With over 365 days
              a year oat origin working with the best growers on the planet,
              only the best beans make the grade.
            </p>
            <v-btn
              v-scroll-reveal.reset="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-10 py-4"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> Shop now
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="shop amber lighten-5 py-12 my-12 text-center">
      <v-container>
        <div class="shop__header mx-auto my-12 py-12 bg-symbol-1">
          <h2 v-scroll-reveal.reset="revealFromBottom" class="overline mb-4">
            Buy now
          </h2>
          <h1 v-scroll-reveal.reset="revealFromBottom" class="display-1">
            Our Best Deal
          </h1>
          <p
            v-scroll-reveal.reset="revealFromBottom"
            class="mt-7 title font-weight-regular mb-12"
          >
            Coffee company with a straightforward mission: to make an ofice and
            on-the-go cup of coffee that we'd like to drink ourselves
          </p>
        </div>
        <v-row align="center" justify="center" no-gutters>
          <v-col lg="4">
            <img
              v-scroll-reveal.reset="revealFromTopWithDelay(100)"
              src="~assets/images/products/amber.png"
              alt=""
            />
            <h4
              v-scroll-reveal.reset="revealFromBottomAt400"
              class="overline my-3"
            >
              Platinum
            </h4>
            <h3 v-scroll-reveal.reset="revealFromBottomAt400" class="title">
              Noansa Platinum Blend
            </h3>
            <v-btn
              v-scroll-reveal.reset="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-7 py-2 mt-3"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> $20.00
            </v-btn>
          </v-col>
          <v-col lg="4">
            <img
              v-scroll-reveal.reset="revealFromTopWithDelay(200)"
              src="~assets/images/products/black.png"
              alt=""
            />
            <h4
              v-scroll-reveal.reset="revealFromBottomAt400"
              class="overline my-3"
            >
              Classic
            </h4>
            <h3 v-scroll-reveal.reset="revealFromBottomAt400" class="title">
              Noansa Classic Blend
            </h3>
            <v-btn
              v-scroll-reveal.reset="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-7 py-2 mt-3"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> $20.00
            </v-btn>
          </v-col>
          <v-col lg="4">
            <img
              v-scroll-reveal.reset="revealFromTopWithDelay(300)"
              src="~assets/images/products/white.png"
              alt=""
            />
            <h4
              v-scroll-reveal.reset="revealFromBottomAt400"
              class="overline my-3"
            >
              General
            </h4>
            <h3 v-scroll-reveal.reset="revealFromBottomAt400" class="title">
              Noansa General Blend
            </h3>
            <v-btn
              v-scroll-reveal.reset="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-7 py-2 mt-3"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> $15.00
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="py-12 my-12">
      <v-container>
        <v-row align="center" no-gutters>
          <v-col lg="6" class="bg-symbol-2">
            <h4 v-scroll-reveal.reset="revealFromBottom" class="overline mb-4">
              Premium Coffee
            </h4>
            <h5 v-scroll-reveal.reset="revealFromBottom" class="display-2">
              The secret lies <br />
              within the bean
            </h5>
            <p
              v-scroll-reveal.reset="revealFromBottom"
              class="title font-weight-regular py-5 pr-10"
            >
              You can't imagine a day without a cup of coffee and we believe
              that your office and on-the-go coffee should never be a
              compromise.
            </p>
            <v-btn
              v-scroll-reveal.reset="revealFromBottomAt400"
              rounded
              height="auto"
              color="primary"
              class="px-10 py-4"
              depressed
            >
              <v-icon left>mdi-hand-pointing-right</v-icon> Shop now
            </v-btn>
          </v-col>
          <v-col lg="6">
            <div
              v-scroll-reveal.reset="revealPointedImg2"
              class="pointed-img-wrap left"
            >
              <v-img
                :src="require('~/assets/images/gallery/pic3.jpg')"
                class="pointed-img"
              ></v-img>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="gallery pt-12 text-center">
      <div class="gallery__header mx-auto bg-symbol-2 pt-12 pb-2 my-12">
        <h1
          v-scroll-reveal.reset="revealFromBottom"
          class="display-2 font-weight-black"
        >
          #NOANSACOFFEE
        </h1>
        <p
          v-scroll-reveal.reset="revealFromBottom"
          class="mx-auto title font-weight-regular mt-2 mb-12"
        >
          Coffee Perfection Since 1927.
        </p>
      </div>
      <v-row no-gutters>
        <v-col v-for="image in gallery" :key="image.id" md="2">
          <v-img
            v-scroll-reveal.reset="revealFromRightWithDelay(image.revealDelay)"
            :src="require(`~/assets/images/gallery/${image.filename}`)"
            aspect-ratio="1"
            class="grey lighten-2"
          ></v-img>
        </v-col>
      </v-row>
    </section>

    <section class="grey darken-3 py-12 white--text text-center">
      <div class="my-12">
        <h1 class="display-2">Would you like to here from us?</h1>
        <p class="mx-auto mt-5 title font-weight-regular">
          Submit your email address for our newsletter
        </p>

        <v-row justify="center" no-gutters>
          <v-col lg="4">
            <v-text-field
              v-model="email"
              label="Your Email address"
              required
              dark
            ></v-text-field>
          </v-col>
        </v-row>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      revealFromBottom: {
        origin: 'bottom',
        distance: '100%'
      },
      revealFromBottomAt400: {
        origin: 'bottom',
        distance: '100%',
        delay: 400
      },
      revealFromRight: {
        distance: '100%',
        origin: 'right'
      },
      revealPointedImg1: {
        distance: '30%',
        origin: 'left'
      },
      revealPointedImg2: {
        distance: '30%',
        origin: 'right'
      },

      gallery: [
        {
          id: 1,
          filename: 'pic1.jpg',
          revealDelay: 100
        },
        {
          id: 2,
          filename: 'pic2.jpg',
          revealDelay: 200
        },
        {
          id: 3,
          filename: 'pic13.jpg',
          revealDelay: 300
        },
        {
          id: 4,
          filename: 'pic4.jpg',
          revealDelay: 400
        },
        {
          id: 5,
          filename: 'pic5.jpg',
          revealDelay: 500
        },
        {
          id: 6,
          filename: 'pic6.jpg',
          revealDelay: 600
        },
        {
          id: 7,
          filename: 'pic7.jpg',
          revealDelay: 700
        },
        {
          id: 8,
          filename: 'pic8.jpg',
          revealDelay: 800
        },
        {
          id: 9,
          filename: 'pic9.jpg',
          revealDelay: 900
        },
        {
          id: 10,
          filename: 'pic10.jpg',
          revealDelay: 1000
        },
        {
          id: 11,
          filename: 'pic11.jpg',
          revealDelay: 1100
        },
        {
          id: 12,
          filename: 'pic12.jpg',
          revealDelay: 1200
        }
      ]
    }
  },

  methods: {
    revealFromRightWithDelay(delay) {
      return {
        distance: '100%',
        origin: 'right',
        delay
      }
    },
    revealFromTopWithDelay(delay) {
      return {
        distance: '50%',
        origin: 'top',
        delay
      }
    }
  }
}
</script>

<style lang="scss">
@import '~vuetify/src/styles/styles.sass';

.bg-symbol-1 {
  position: relative;
  z-index: 2;

  &::before {
    background-image: url(~assets/images/symbol-bg1.png);
    background-repeat: no-repeat;
    width: 470px;
    height: 400px;
    content: '';
    position: absolute;
    z-index: -1;
    top: -75px;
    left: 100px;
  }
}
.bg-symbol-2 {
  position: relative;
  z-index: 2;

  &::before {
    background-image: url(~assets/images/symbol-bg2.png);
    background-repeat: no-repeat;
    width: 470px;
    height: 400px;
    content: '';
    position: absolute;
    z-index: -1;
    top: -125px;
    left: -50px;
  }
}

.hero {
  background-color: #f3f0e6;
  height: 590px;
  padding-top: 85px;
  position: relative;

  .hero__image {
    position: relative;
    top: -117px;
    right: -100px;
  }

  .hero__dots {
    position: absolute;
    right: 0;
    bottom: -100px;
    height: 205px;
    width: 200px;
    margin-left: auto;
    background-image: url(~assets/images/dots.png);
  }

  .bg-symbol-1 {
    &::before {
      background-image: url(~assets/images/symbol-bg-hero.png);
      left: -240px;
      top: -135px;
    }
  }
}

.icon-box {
  width: 250px;
  margin-right: 20px;
  padding: 40px;
  position: relative;
  overflow: hidden;
  border-radius: 0 60px 0 0;

  .icon-box__icon {
    position: relative;
    z-index: 2;
    padding-top: 25px;
  }

  &:hover {
    background-color: rgba(map-get($amber, 'darken-1'), 0.1);
  }

  &:first-of-type {
    background-color: rgba(map-get($amber, 'darken-1'), 0.2);

    &::before {
      content: '';
      position: absolute;
      z-index: 1;
      top: -60px;
      left: -40px;
      width: 125%;
      height: 178px;
      background-color: map-get($amber, 'darken-1');
      border-radius: 50%;
    }
  }
}

.shop {
  position: relative;

  .shop__header {
    width: 60%;

    &::before {
      background-image: url(~assets/images/symbol-bg-shop.png);
    }
  }

  &::after {
    content: '';
    position: absolute;
    bottom: -100px;
    left: 0;
    height: 205px;
    width: 200px;
    background-image: url(~assets/images/dots.png);
  }
}

.pointed-img-wrap {
  position: relative;

  &::before {
    position: absolute;
    left: -50px;
    content: '';
    height: 205px;
    width: 200px;
    background-image: url(~assets/images/dots.png);
  }

  &::after {
    content: '';
    position: absolute;
    bottom: -67px;
    right: 130px;
    width: 40px;
    height: 200px;
    background-color: rgba(map-get($amber, 'darken-1'), 0.7);
    border-radius: 20px;
    transform: rotate(45deg);
  }

  .pointed-img {
    height: 470px;
    width: 470px;
    border-radius: 50% 50% 0 50%;
  }

  &.left {
    .pointed-img {
      border-radius: 50% 50% 50% 0;
    }

    &::before {
      left: initial;
      right: 55px;
    }

    &::after {
      transform: rotate(-45deg);
      right: initial;
      left: 20px;
    }
  }
}

.gallery {
  .gallery__header {
    width: 30%;
  }
}
</style>
