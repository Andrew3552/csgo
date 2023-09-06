<template>
  <div :class="$style.head">
    <picture :class="$style.image">
      <source media="(max-width: 768px)" srcset="/images/head-2.png" />
      <source media="(min-width: 769px)" srcset="/images/head-1.png" />
      <img src="/images/head-2.png" />
    </picture>

    <div :class="$style.content">
      <div :class="$style.underTitle">{{ $t('header.note') }}</div>

      <div :class="$style.title" v-if="locale === 'tr'">
        <span>{{ $t('header.title.part1')}}&nbsp;</span>{{ $t('header.title.part2')}}<br>{{ $t('header.title.part3')}}
      </div>
      <div :class="$style.title" v-if="locale !== 'tr'">
        {{ $t('header.title.part1')}}<br>{{ $t('header.title.part2')}}<br><span>{{ $t('header.title.part3')}}</span>
      </div>

      <p>
        {{ $t('header.description')}}
      </p>
      <a href="/" :class="$style.button">
        <svg width="293" height="82" viewBox="0 0 293 82" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M146.212 11.8076H14.2115V40.9999L23.7308 54.3268L35.7885 70.8268L146.212 70.8269H278.212V41.6346L268.692 28.3077L256.635 11.8077H146.212V11.8076Z" fill="url(#paint0_linear_8_26)"/>
          <g filter="url(#filter0_f_8_26)">
          <mask id="path-2-inside-1_8_26" fill="white">
          <path d="M146.212 74H284.558V41.3548L274.581 26.4516L261.943 8H146.212H8.5V41L30.7115 74H146.212Z"/>
          </mask>
          <path d="M284.558 74V75H285.558V74H284.558ZM274.581 26.4516L275.412 25.8953L275.406 25.8866L274.581 26.4516ZM284.558 41.3548H285.558V41.051L285.389 40.7985L284.558 41.3548ZM261.943 8L262.768 7.43493L262.471 7H261.943V8ZM8.5 8V7H7.5V8H8.5ZM8.5 41H7.5V41.3052L7.67041 41.5584L8.5 41ZM30.7115 74L29.8819 74.5584L30.1792 75H30.7115V74ZM284.558 73H146.212V75H284.558V73ZM273.75 27.0079L283.727 41.9111L285.389 40.7985L275.412 25.8953L273.75 27.0079ZM283.558 41.3548V74H285.558V41.3548H283.558ZM146.212 9H261.943V7H146.212V9ZM261.118 8.56507L273.756 27.0167L275.406 25.8866L262.768 7.43493L261.118 8.56507ZM146.212 7H8.5V9H146.212V7ZM7.5 8V41H9.5V8H7.5ZM7.67041 41.5584L29.8819 74.5584L31.5411 73.4416L9.32959 40.4416L7.67041 41.5584ZM30.7115 75H146.212V73H30.7115V75Z" fill="url(#paint1_linear_8_26)" mask="url(#path-2-inside-1_8_26)"/>
          </g>
          <mask id="path-4-inside-2_8_26" fill="white">
          <path d="M146.212 74H284.558V41.3548L274.581 26.4516L261.943 8H146.212H8.5V41L30.7115 74H146.212Z"/>
          </mask>
          <path d="M284.558 74V75H285.558V74H284.558ZM274.581 26.4516L275.412 25.8953L275.406 25.8866L274.581 26.4516ZM284.558 41.3548H285.558V41.051L285.389 40.7985L284.558 41.3548ZM261.943 8L262.768 7.43493L262.471 7H261.943V8ZM8.5 8V7H7.5V8H8.5ZM8.5 41H7.5V41.3052L7.67041 41.5584L8.5 41ZM30.7115 74L29.8819 74.5584L30.1792 75H30.7115V74ZM284.558 73H146.212V75H284.558V73ZM273.75 27.0079L283.727 41.9111L285.389 40.7985L275.412 25.8953L273.75 27.0079ZM283.558 41.3548V74H285.558V41.3548H283.558ZM146.212 9H261.943V7H146.212V9ZM261.118 8.56507L273.756 27.0167L275.406 25.8866L262.768 7.43493L261.118 8.56507ZM146.212 7H8.5V9H146.212V7ZM7.5 8V41H9.5V8H7.5ZM7.67041 41.5584L29.8819 74.5584L31.5411 73.4416L9.32959 40.4416L7.67041 41.5584ZM30.7115 75H146.212V73H30.7115V75Z" fill="url(#paint2_linear_8_26)" mask="url(#path-4-inside-2_8_26)"/>
          <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" fill="white">{{ $t('header.button')}}</text>
          <defs>
          <filter id="filter0_f_8_26" x="0.5" y="0" width="292.058" height="82" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
          <feFlood flood-opacity="0" result="BackgroundImageFix"/>
          <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
          <feGaussianBlur stdDeviation="4" result="effect1_foregroundBlur_8_26"/>
          </filter>
          <linearGradient id="paint0_linear_8_26" x1="21.1923" y1="50.5192" x2="278.212" y2="40.9999" gradientUnits="userSpaceOnUse">
          <stop stop-color="#FF552E"/>
          <stop offset="1" stop-color="#FF0000"/>
          </linearGradient>
          <linearGradient id="paint1_linear_8_26" x1="284.558" y1="74" x2="-84.1539" y2="-18.6538" gradientUnits="userSpaceOnUse">
          <stop stop-color="#FF552E"/>
          <stop offset="1" stop-color="#FF552E" stop-opacity="0"/>
          </linearGradient>
          <linearGradient id="paint2_linear_8_26" x1="284.558" y1="74" x2="-84.1539" y2="-18.6538" gradientUnits="userSpaceOnUse">
          <stop stop-color="#FF552E"/>
          <stop offset="1" stop-color="#FF552E" stop-opacity="0"/>
          </linearGradient>
          </defs>
        </svg>
      </a>
    </div>
  </div>
</template>

<script lang="ts" setup>
import {useI18n} from "vue-i18n";

const {locale} = useI18n();
</script>

<style lang="scss" module>
  .head {
    position: relative;
    display: flex;
    align-items: center;
    min-height: calc(100vh - 82px);

    @media (max-width: 768px) {
      min-height: calc(100vh - 61px);
    }

    @media (max-width: 550px) {
      align-items: flex-end;
    }
  }

  .image {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: right;

      @media (max-width: 550px) {
        object-position: 75% center;
      }
    }
  }

  .content {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 110px 0 110px 93px;

    @media (max-width: 768px) {
      padding: 100px 0 100px 24px;
    }

    @media (max-width: 550px) {
      justify-content: flex-end;
      padding: 0 0 132px 16px;
    }
  }

  .underTitle {
    font-family: 'Wadik';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 22px;
    color: #FF552E;

    @media (max-width: 768px) {
      font-size: 12px;
      line-height: 13px;
    }
  }

  .title {
    font-family: 'Wadik';
    font-style: normal;
    font-weight: 700;
    font-size: 90px;
    line-height: 100px;
    color: #FFFFFF;

    @media (max-width: 768px) {
      font-size: 32px;
      line-height: 35px;
    }

    span {
      color: #FF552E;
    }
  }

  p {
    margin: 50px 0 0 0;
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    color: #FFFFFF;
    max-width: 655px;

    @media (max-width: 768px) {
      margin: 25px 0 0 0;
      max-width: 335px;
      font-size: 14px;
      line-height: 17px;
    }
  }

  .button {
    display: inline-block;
    margin-top: 50px;

    @media (max-width: 768px) {
      margin-top: 30px;

      svg {
        width: 220px !important;
        height: auto !important;
      }
    }
    cursor: pointer;
    text-decoration: none;
    transition: 200ms ease-in-out;

    &:hover {
      opacity: 0.7;
    }
  }
</style>
