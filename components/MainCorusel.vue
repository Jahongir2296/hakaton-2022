<template>
  <div class="carousel">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h3 class="carousel__title">
            {{ "carousel.title" }}
          </h3>
        </div>
        <div
          data-aos="fade-up"
          data-aos-easing="linear"
          data-aos-duration="1500"
          data-aos-once="true"
          class="carousel__texts col-12 d-flex justify-content-between align-items-center"
        >
          <p class="carousel__subtitle">
            {{ "carousel.subtitle_yuridik" }}
          </p>
          <div class="d-flex align-items-center">
            <div class="ml-5">
              <button @click="showPrev">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M3.35288 8.95043C4.00437 6.17301 6.17301 4.00437 8.95043 3.35288C10.9563 2.88237 13.0437 2.88237 15.0496 3.35288C17.827 4.00437 19.9956 6.17301 20.6471 8.95044C21.1176 10.9563 21.1176 13.0437 20.6471 15.0496C19.9956 17.827 17.827 19.9956 15.0496 20.6471C13.0437 21.1176 10.9563 21.1176 8.95044 20.6471C6.17301 19.9956 4.00437 17.827 3.35288 15.0496C2.88237 13.0437 2.88237 10.9563 3.35288 8.95043Z"
                    stroke="white"
                    stroke-width="1.5"
                  />
                  <path
                    d="M13 14.5L10.5 12L13 9.5"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
              <button @click="showNext">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M3.35288 8.95043C4.00437 6.17301 6.17301 4.00437 8.95043 3.35288C10.9563 2.88237 13.0437 2.88237 15.0496 3.35288C17.827 4.00437 19.9956 6.17301 20.6471 8.95044C21.1176 10.9563 21.1176 13.0437 20.6471 15.0496C19.9956 17.827 17.827 19.9956 15.0496 20.6471C13.0437 21.1176 10.9563 21.1176 8.95044 20.6471C6.17301 19.9956 4.00437 17.827 3.35288 15.0496C2.88237 13.0437 2.88237 10.9563 3.35288 8.95043Z"
                    stroke="white"
                    stroke-width="1.5"
                  />
                  <path
                    d="M11 9.5L13.5 12L11 14.5"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
        <div
          class="col-12 mb-6"
          data-aos="fade-up"
          data-aos-easing="linear"
          data-aos-duration="1500"
          data-aos-once="true"
        >
          <VueSlickCarousel v-bind="settings" ref="carousel" class="">
            <a
              v-for="item in carouselComponent"
              :key="item.id"
              draggable="false"
              ondragstart="return false"
              href="https://uic.group/uz"
              class="carousel__item d-flex align-items-center justify-content-betweem"
            >
              <img
                draggable="false"
                ondragstart="return false"
                :src="item.image"
                :alt="item.name"
              />
              <img
                draggable="false"
                ondragstart="return false"
                :src="item.hover_image"
                :alt="item.name"
              />
            </a>
          </VueSlickCarousel>
        </div>
        <p
          class="col-12 carousel__subtitle carousel__subtitle-2"
          data-aos="fade-up"
          data-aos-easing="linear"
          data-aos-duration="1500"
          data-aos-once="true"
        >
          {{"carousel.subtitle_jismoniy" }}
        </p>
      </div>
    </div>

    <div
      class="carousel-rows"
      data-aos="fade-up"
      data-aos-easing="linear"
      data-aos-duration="1500"
      data-aos-once="true"
    >
      <!-- <VueSlickCarousel v-bind="settings2">
        <div
          v-for="item in carouselPlanted"
          :key="item.id"
          class="carousel-rows__item rows-item"
        >
          <div class="rows-item__top d-flex align-items-center">
            <img
              draggable="false"
              ondragstart="return false"
              :src="item.image"
              alt="user"
            />
            <a
              :href="item.account_link"
              target="_blank"
              draggable="false"
              ondragstart="return false"
            >
              <p class="name">{{ item.name }}</p>
              <span class="d-flex align-items-center">
                <svg
                  v-if="item.type === 1"
                  width="14"
                  height="14"
                  viewBox="0 0 14 14"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M7.01648 0.633057C5.2828 0.633057 5.06542 0.640404 4.38455 0.671471C3.7051 0.702461 3.24105 0.81038 2.83501 0.968195C2.41523 1.1313 2.05924 1.34958 1.70434 1.70446C1.34946 2.05936 1.13118 2.41536 0.968072 2.83513C0.810258 3.24117 0.702343 3.70521 0.671353 4.38467C0.640286 5.06554 0.632935 5.28292 0.632935 7.0166C0.632935 8.75025 0.640286 8.96764 0.671353 9.64851C0.702343 10.328 0.810258 10.792 0.968072 11.198C1.13118 11.6178 1.34946 11.9738 1.70434 12.3287C2.05924 12.6836 2.41523 12.9019 2.83501 13.065C3.24105 13.2228 3.7051 13.3307 4.38455 13.3617C5.06542 13.3928 5.2828 13.4001 7.01648 13.4001C8.75013 13.4001 8.96751 13.3928 9.64838 13.3617C10.3278 13.3307 10.7919 13.2228 11.1979 13.065C11.6177 12.9019 11.9737 12.6836 12.3286 12.3287C12.6835 11.9738 12.9017 11.6178 13.0649 11.198C13.2227 10.792 13.3306 10.328 13.3616 9.64851C13.3926 8.96764 13.4 8.75025 13.4 7.0166C13.4 5.28292 13.3926 5.06554 13.3616 4.38467C13.3306 3.70521 13.2227 3.24117 13.0649 2.83513C12.9017 2.41536 12.6835 2.05936 12.3286 1.70446C11.9737 1.34958 11.6177 1.1313 11.1979 0.968195C10.7919 0.81038 10.3278 0.702461 9.64838 0.671471C8.96751 0.640404 8.75013 0.633057 7.01648 0.633057ZM7.01648 1.78324C8.72094 1.78324 8.92284 1.78975 9.59596 1.82046C10.2183 1.84884 10.5564 1.95284 10.7813 2.04026C11.0793 2.15606 11.2919 2.29439 11.5153 2.51778C11.7387 2.74115 11.877 2.9538 11.9928 3.25176C12.0802 3.4767 12.1842 3.81471 12.2126 4.43709C12.2433 5.11021 12.2498 5.31212 12.2498 7.0166C12.2498 8.72106 12.2433 8.92296 12.2126 9.59608C12.1842 10.2185 12.0802 10.5565 11.9928 10.7814C11.877 11.0794 11.7387 11.292 11.5153 11.5154C11.2919 11.7388 11.0793 11.8771 10.7813 11.9929C10.5564 12.0803 10.2183 12.1843 9.59596 12.2127C8.92294 12.2434 8.72107 12.2499 7.01648 12.2499C5.31187 12.2499 5.11001 12.2434 4.43697 12.2127C3.81458 12.1843 3.47658 12.0803 3.25164 11.9929C2.95368 11.8771 2.74102 11.7388 2.51766 11.5154C2.29429 11.292 2.15594 11.0794 2.04014 10.7814C1.95271 10.5565 1.84872 10.2185 1.82034 9.59608C1.78963 8.92296 1.78312 8.72106 1.78312 7.0166C1.78312 5.31212 1.78963 5.11021 1.82034 4.43709C1.84872 3.81471 1.95271 3.4767 2.04014 3.25176C2.15594 2.9538 2.29426 2.74115 2.51766 2.51778C2.74102 2.29439 2.95368 2.15606 3.25164 2.04026C3.47658 1.95284 3.81458 1.84884 4.43697 1.82046C5.11009 1.78975 5.312 1.78324 7.01648 1.78324ZM7.01648 3.73856C5.20605 3.73856 3.73844 5.20617 3.73844 7.0166C3.73844 8.827 5.20605 10.2946 7.01648 10.2946C8.82688 10.2946 10.2945 8.827 10.2945 7.0166C10.2945 5.20617 8.82688 3.73856 7.01648 3.73856ZM7.01648 9.14443C5.84129 9.14443 4.88862 8.19177 4.88862 7.0166C4.88862 5.84141 5.84129 4.88874 7.01648 4.88874C8.19165 4.88874 9.14431 5.84141 9.14431 7.0166C9.14431 8.19177 8.19165 9.14443 7.01648 9.14443ZM11.19 3.60905C11.19 4.03212 10.8471 4.37506 10.424 4.37506C10.001 4.37506 9.65799 4.03212 9.65799 3.60905C9.65799 3.18598 10.001 2.84301 10.424 2.84301C10.8471 2.84301 11.19 3.18598 11.19 3.60905Z"
                    fill="#A5ABAA"
                  />
                </svg>
                <svg
                  v-if="item.type === 2"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g opacity="0.5">
                    <path
                      d="M12.5413 10.875L12.9043 8.34133H10.6347V6.69715C10.6347 6.00398 10.9517 5.32832 11.9682 5.32832H13V3.17117C13 3.17117 12.0637 3 11.1684 3C9.29936 3 8.07764 4.21352 8.07764 6.41031V8.34133H6V10.875H8.07764V17H10.6347V10.875H12.5413Z"
                      fill="white"
                    />
                  </g>
                </svg>
                <svg
                  v-if="item.type === 3"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g opacity="0.5">
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M18 4.57843C17.4121 4.84616 16.7791 5.02721 16.1152 5.1081C16.7932 4.69207 17.3135 4.03238 17.5586 3.24654C16.9238 3.63176 16.2222 3.912 15.4728 4.06224C14.8755 3.40833 14.0218 3 13.0771 3C11.2655 3 9.79574 4.50716 9.79574 6.36583C9.79574 6.62971 9.82391 6.88588 9.88026 7.13242C7.15208 6.99182 4.73381 5.65318 3.11381 3.61442C2.83113 4.11328 2.6696 4.69207 2.6696 5.30842C2.6696 6.47562 3.24905 7.50608 4.12995 8.10991C3.59277 8.09354 3.08563 7.94041 2.64236 7.69002V7.73143C2.64236 9.36283 3.77402 10.7236 5.27663 11.0318C5.00147 11.1107 4.71128 11.1502 4.41169 11.1502C4.20039 11.1502 3.99378 11.13 3.79374 11.0905C4.21166 12.4272 5.42313 13.4009 6.86001 13.4269C5.7368 14.3302 4.32059 14.8685 2.78323 14.8685C2.5184 14.8685 2.25638 14.8531 2 14.8223C3.45284 15.7757 5.17896 16.3333 7.03187 16.3333C13.0705 16.3333 16.3715 11.2051 16.3715 6.75683C16.3715 6.61045 16.3687 6.46407 16.3631 6.32057C17.0045 5.84579 17.5614 5.25352 18 4.57843Z"
                      fill="white"
                    />
                  </g>
                </svg>
                <svg
                  v-if="item.type === 4"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >$
                  <g opacity="0.5" clip-path="url(#clip0)">
                    <path
                      d="M19.9471 4.15771L17.1446 16.2805C16.9331 17.1361 16.3817 17.3491 15.5982 16.946L11.328 14.0598L9.26758 15.8775C9.03956 16.0866 8.84885 16.2615 8.4094 16.2615L8.71619 12.2726L16.6305 5.71299C16.9746 5.43159 16.5559 5.27568 16.0957 5.55708L6.31164 11.2078L2.09953 9.99857C1.18331 9.73619 1.16673 9.15819 2.29023 8.75511L18.7656 2.93325C19.5284 2.67087 20.1958 3.08916 19.9471 4.15771Z"
                      fill="white"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0">
                      <rect width="20" height="20" fill="white" />
                    </clipPath>
                  </defs>
                </svg>
                <p class="username">@{{ item.username }}</p>
              </span>
            </a>
          </div>
          <img
            draggable="false"
            ondragstart="return false"
            class="rows-item__img img-fluid"
            :src="item.image"
            alt=""
          />
        </div>
      </VueSlickCarousel> -->
      <div class="carousel__gradient"></div>
    </div>

    <div class="container">
      <div class="row">
        <nuxt-link
          :to="`/plant-tree`"
          class="col-10 col-lg-8 col-md-5 mx-auto carousel__link"
        >
          <button class="">
            {{ "carousel.link" }}
          </button>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  components: {
    VueSlickCarousel,
  },
  data() {
    return {
      items: [
        {
          image:"../static/corusel/UIC-logo.png"
        },
         {
          image:"../static/corusel/UIC-logo.png"
        },
         {
          image:"../static/corusel/UIC-logo.png"
        },
         {
          image:"../static/corusel/UIC-logo.png"
        },
         {
          image:"../static/corusel/UIC-logo.png"
        },
         {
          image:"../static/corusel/UIC-logo.png"
        },
      ],
      settings: {
        dots: true,
        focusOnSelect: false,
        infinite: true,
        speed: 500,
        slidesToShow: 4,
        slidesToScroll: 1,
        arrows: false,
        dotsClass: "slick-dots",
        autoplay: true,
        autoplaySpeed: 5000,
        responsive: [
          {
            breakpoint: 800,
            settings: {
              slidesToShow: 3,
            },
          },
          {
            breakpoint: 576,
            settings: {
              slidesToShow: 2,
            },
          },
        ],
      },
      settings2: {
        infinite: true,
        slidesToShow: 14,
        speed: 500,
        rows: 3,
        slidesPerRow: 1,
        autoplay: false,
        autoplaySpeed: 2000,
        responsive: [
          {
            breakpoint: 1000,
            settings: {
              slidesToShow: 10,
            },
          },
          {
            breakpoint: 850,
            settings: {
              slidesToShow: 8,
            },
          },
          {
            breakpoint: 750,
            settings: {
              slidesToShow: 7,
            },
          },
          {
            breakpoint: 500,
            settings: {
              slidesToShow: 5,
            },
          },
          {
            breakpoint: 450,
            settings: {
              slidesToShow: 4,
            },
          },
          {
            breakpoint: 373,
            settings: {
              slidesToShow: 3,
            },
          },
        ],
      },
    };
  },
  methods: {
    showNext() {
      this.$refs.carousel.next();
    },
    showPrev() {
      this.$refs.carousel.prev();
    },
  },
};
</script>

<style lang="scss">
.carousel {
  margin-top: 64px;
  margin-bottom: 128px;
  &__title {
    font-size: 36px;
    line-height: 45px;
    font-weight: bold;
  }
  &__texts {
    margin: 24px 0 16px;
    position: relative;
  }
  &__subtitle {
    font-weight: 500;
    font-size: 24px;
    // margin: 24px 0 16px;
  }
  &__subtitle-2 {
    margin-top: 24px;
  }
  &__item {
    width: 90% !important;
    margin: 0 auto;
    height: 168px;
    background: #1c2b27;
    border: 1px solid #a5abaa;
    border-radius: 16px;
    display: flex !important;
    align-items: center;
    justify-content: center;
    transition: all 0.6s;
    position: relative;

    &:hover {
      background: #121f1b;
      border: 1px solid #188859;

      img:nth-child(1) {
        opacity: 0;
      }
      img:nth-child(2) {
        opacity: 1;
      }
    }

    img {
      width: 50%;
      max-height: 60px;
      position: absolute;
      transition: all 0.6s;
    }
    img:nth-child(1) {
      opacity: 1;
    }
    img:nth-child(2) {
      opacity: 0;
    }
  }
  .slick-dots {
    position: absolute;
    top: -48px;
    right: -42%;
    pointer-events: none;

    @media (max-width: 1040px) {
      right: -40%;
    }
    @media (max-width: 880px) {
      right: -39%;
    }
    @media (max-width: 812px) {
      right: -38%;
    }
    @media (max-width: 720px) {
      right: -37%;
    }
    @media (max-width: 675px) {
      right: -36%;
    }
    @media (max-width: 650px) {
      right: -34%;
    }
    @media (max-width: 550px) {
      right: -32%;
    }
    @media (max-width: 510px) {
      right: -28%;
    }
    @media (max-width: 420px) {
      right: -25%;
    }
    @media (max-width: 380px) {
      right: -22%;
      top: -47px;
    }

    li {
      width: 4px;
    }

    li button::before {
      color: #fff;
      width: 10px;
      height: 10px;
      font-size: 8px;
    }
  }
  .carousel-rows {
    position: relative;
    z-index: 10;
    height: 350px;
    overflow: hidden;

    @media (max-width: 470px) {
      // max-height: 300px;
    }
    .rows-item__img {
      width: 100px;
      height: 100px;
    }

    .slick-slide {
      margin: 0px 2px;
      & > div {
        margin: -4px auto;
      }

      @media (max-width: 1800px) {
        margin: 0 -14px;
      }
      @media (max-width: 1750px) {
        margin: 0 -12px;
      }
      @media (max-width: 1700px) {
        margin: 0 -10px;
      }
      @media (max-width: 1650px) {
        margin: 0 -8px;
      }
      @media (max-width: 1600px) {
        margin: 0 -6px;
      }
      @media (max-width: 1550px) {
        margin: 0 -4px;
      }
      @media (max-width: 1500px) {
        margin: 0 -2px;
      }
      @media (max-width: 1476px) {
        margin: 0 -1px;
      }
      @media (max-width: 1210px) {
        margin: 0 2px;
      }
      @media (max-width: 850px) {
        margin: 0 -3px;
      }
    }
    .slick-track {
      padding-top: 30px;
      z-index: 10;
    }
    &__item {
      position: relative;
      z-index: 2;

      &:hover {
        z-index: 23;
        cursor: pointer;
      }

      &:hover .rows-item__top {
        opacity: 1;
      }

      .carousel-rows__img {
        z-index: 10;
      }

      .rows-item__top {
        opacity: 0;
        position: absolute;
        top: -20px;
        z-index: 500;
        transform: translateX(-30%);
        background-color: #020b09;
        padding: 8px;
        border-radius: 8px;
        transition: 0.3s;

        img {
          display: block;
          width: 36px;
          height: 36px;
          border-radius: 4px;
          margin-right: 8px;
        }
        .name {
          white-space: nowrap;
          color: #fff;
        }
        .username {
          color: #a5abaa;
          font-size: 12px;
          margin-left: 5px;
        }
      }
    }
  }
  &__gradient {
    position: absolute;
    top: 0;
    bottom: -10px;
    right: 0;
    left: 0;
    background-image: linear-gradient(
      180deg,
      rgba(255, 255, 255, 0) 9%,
      rgba(209, 212, 212, 0) 51%,
      rgba(3, 20, 16, 1) 89%,
      rgba(3, 20, 16, 1) 98%,
      rgba(3, 20, 16, 1) 100%
    );
    pointer-events: none;
  }

  &__link button {
    width: 100%;
    background: #188859;
    color: #fff;
    text-align: center;
    font-weight: bold;
    font-size: 24px;
    line-height: 30px;
    border-radius: 8px;
    padding: 16px 0;
    margin-top: 16px;
    cursor: pointer;
    transition: 0.2s ease;

    @media (max-width: 576px) {
      margin-top: 0px;
      font-size: 20px;
    }

    &:hover {
      background-color: #16734c;
      color: #fff;
    }
  }
}
</style>
