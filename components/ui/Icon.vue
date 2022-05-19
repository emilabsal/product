<template>
  <svg
    v-if="name === 'theme'"
    :width="width ? width : 32"
    :height="height ? height : 32"
    viewBox="0 0 32 32"
    fill=""
    xmlns="http://www.w3.org/2000/svg"
  >
    <rect
      :width="width ? width : 32"
      :height="height ? height : 32"
      rx="16"
      fill="#F3F3F3"
    />
    <path
      d="M16 26C21.514 26 26 21.514 26 16C26 10.486 21.514 6 16 6C10.486 6 6 10.486 6 16C6 21.514 10.486 26 16 26ZM16 8C20.411 8 24 11.589 24 16C24 20.411 20.411 24 16 24C11.589 24 8 20.411 8 16C8 11.589 11.589 8 16 8Z"
      :fill="fill ? fill : '#02897A'"
    />
    <path
      d="M23 16C23 12.134 19.865 9 16 9V23C19.865 23 23 19.866 23 16Z"
      :fill="fill ? fill : '#02897A'"
    />
  </svg>
  <svg
    v-else-if="name === 'instagram'"
    :width="width ? width : 24"
    :height="height ? height : 25"
    viewBox="0 0 24 25"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M17 2.01611H7C4.23858 2.01611 2 4.25469 2 7.01611V17.0161C2 19.7775 4.23858 22.0161 7 22.0161H17C19.7614 22.0161 22 19.7775 22 17.0161V7.01611C22 4.25469 19.7614 2.01611 17 2.01611Z"
      :stroke="fill ? fill : '#02897A'"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M16 11.3859C16.1234 12.2182 15.9812 13.0681 15.5937 13.8149C15.2062 14.5617 14.5931 15.1673 13.8416 15.5456C13.0901 15.9239 12.2384 16.0555 11.4077 15.9219C10.5771 15.7882 9.80971 15.396 9.21479 14.8011C8.61987 14.2062 8.22768 13.4388 8.09402 12.6081C7.96035 11.7775 8.09202 10.9258 8.47028 10.1743C8.84854 9.42278 9.45414 8.80967 10.2009 8.42217C10.9477 8.03467 11.7977 7.89251 12.63 8.01593C13.4789 8.14181 14.2648 8.53739 14.8716 9.14423C15.4785 9.75108 15.8741 10.537 16 11.3859Z"
      :stroke="fill ? fill : '#02897A'"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M17.5 6.51611H17.51"
      :stroke="fill ? fill : '#02897A'"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
  <svg
    v-else-if="name === 'facebook'"
    :width="width ? width : 24"
    :height="height ? height : 24"
    viewBox="0 0 24 24"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M18 2H15C13.6739 2 12.4021 2.52678 11.4645 3.46447C10.5268 4.40215 10 5.67392 10 7V10H7V14H10V22H14V14H17L18 10H14V7C14 6.73478 14.1054 6.48043 14.2929 6.29289C14.4804 6.10536 14.7348 6 15 6H18V2Z"
      :stroke="fill ? fill : '#02897A'"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
  <svg
    v-else-if="name === 'twitter'"
    :width="width ? width : 24"
    :height="height ? height : 20"
    viewBox="0 0 24 20"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M23 1.01006C22.0424 1.68553 20.9821 2.20217 19.86 2.54006C19.2577 1.84757 18.4573 1.35675 17.567 1.13398C16.6767 0.911216 15.7395 0.967251 14.8821 1.29451C14.0247 1.62177 13.2884 2.20446 12.773 2.96377C12.2575 3.72309 11.9877 4.62239 12 5.54006V6.54006C10.2426 6.58562 8.50127 6.19587 6.93101 5.4055C5.36074 4.61513 4.01032 3.44869 3 2.01006C3 2.01006 -1 11.0101 8 15.0101C5.94053 16.408 3.48716 17.109 1 17.0101C10 22.0101 21 17.0101 21 5.51006C20.9991 5.23151 20.9723 4.95365 20.92 4.68006C21.9406 3.67355 22.6608 2.40277 23 1.01006V1.01006Z"
      :stroke="fill ? fill : '#02897A'"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
  <svg
    v-else-if="name === 'play'"
    :width="width ? width : 17"
    :height="height ? height : 19"
    viewBox="0 0 17 19"
    fill=""
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      fill-rule="evenodd"
      clip-rule="evenodd"
      d="M15.8516 8.53032C16.591 8.96531 16.591 10.0347 15.8516 10.4697L2.1954 18.5027C1.44543 18.9439 0.5 18.4031 0.5 17.533V1.46697C0.5 0.596876 1.44543 0.0561381 2.1954 0.497293L15.8516 8.53032Z"
      :fill="fill ? fill : '#02897A'"
    />
  </svg>
  <svg
    v-else-if="name === 'click'"
    :width="width ? width : 58"
    :height="height ? height : 59"
    viewBox="0 0 58 59"
    fill=""
    xmlns="http://www.w3.org/2000/svg"
  >
    <g clip-path="url(#clip0_1_541)" filter="url(#filter0_d_1_541)">
      <rect x="4" y="0.830078" width="50" height="50" rx="19" fill="#02897A" />
      <path
        d="M33.1161 27.4283L23.9732 18.2854C23.8661 18.1694 23.7232 18.1158 23.5714 18.1158C23.5 18.1158 23.4196 18.1336 23.3571 18.1604C23.1429 18.2497 23 18.4551 23 18.6872V32.1158C23 32.3479 23.1429 32.5533 23.3571 32.6426C23.4196 32.6694 23.5 32.6872 23.5714 32.6872C23.7232 32.6872 23.8661 32.6247 23.9732 32.5176L26.7589 29.7319L28.4643 33.7676C28.5893 34.0533 28.9196 34.1961 29.2143 34.0711L30.7946 33.4015C31.0804 33.2765 31.2232 32.9461 31.0982 32.6515L29.3036 28.4015H32.7143C32.9464 28.4015 33.1518 28.2586 33.2411 28.0444C33.3304 27.839 33.2857 27.589 33.1161 27.4283Z"
        fill="white"
      />
    </g>
    <defs>
      <filter
        id="filter0_d_1_541"
        x="0"
        y="0.830078"
        width="59"
        height="58"
        filterUnits="userSpaceOnUse"
        color-interpolation-filters="sRGB"
      >
        <feFlood flood-opacity="0" result="BackgroundImageFix" />
        <feColorMatrix
          in="SourceAlpha"
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
          result="hardAlpha"
        />
        <feOffset dy="4" />
        <feGaussianBlur stdDeviation="2" />
        <feColorMatrix
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
        />
        <feBlend
          mode="normal"
          in2="BackgroundImageFix"
          result="effect1_dropShadow_1_541"
        />
        <feBlend
          mode="normal"
          in="SourceGraphic"
          in2="effect1_dropShadow_1_541"
          result="shape"
        />
      </filter>
      <clipPath id="clip0_1_541">
        <rect
          width="51"
          height="50"
          fill="white"
          transform="translate(4 0.830078)"
        />
      </clipPath>
    </defs>
  </svg>
  <svg
    v-else-if="name === 'design'"
    :width="width ? width : 50"
    :height="height ? height : 51"
    viewBox="0 0 50 51"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <rect y="0.830078" width="50" height="50" rx="19" fill="#4D8DFF" />
  </svg>
  <svg
    v-else-if="name === 'preference'"
    :width="width ? width : 58"
    :height="height ? height : 59"
    viewBox="0 0 58 59"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <g clip-path="url(#clip0_1_557)" filter="url(#filter0_d_1_557)">
      <rect x="4" y="0.830078" width="50" height="50" rx="19" fill="#740A76" />
      <path
        d="M29 33.9729C29.1429 33.9729 29.2857 33.9194 29.3929 33.8122L34.9554 28.4551C35.0357 28.3747 37 26.5801 37 24.4372C37 21.8211 35.4018 20.2586 32.7321 20.2586C31.1696 20.2586 29.7054 21.4908 29 22.1872C28.2946 21.4908 26.8304 20.2586 25.2679 20.2586C22.5982 20.2586 21 21.8211 21 24.4372C21 26.5801 22.9643 28.3747 23.0357 28.4372L28.6071 33.8122C28.7143 33.9194 28.8571 33.9729 29 33.9729Z"
        fill="white"
      />
    </g>
    <defs>
      <filter
        id="filter0_d_1_557"
        x="0"
        y="0.830078"
        width="58"
        height="58"
        filterUnits="userSpaceOnUse"
        color-interpolation-filters="sRGB"
      >
        <feFlood flood-opacity="0" result="BackgroundImageFix" />
        <feColorMatrix
          in="SourceAlpha"
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
          result="hardAlpha"
        />
        <feOffset dy="4" />
        <feGaussianBlur stdDeviation="2" />
        <feColorMatrix
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
        />
        <feBlend
          mode="normal"
          in2="BackgroundImageFix"
          result="effect1_dropShadow_1_557"
        />
        <feBlend
          mode="normal"
          in="SourceGraphic"
          in2="effect1_dropShadow_1_557"
          result="shape"
        />
      </filter>
      <clipPath id="clip0_1_557">
        <rect
          width="50"
          height="50"
          fill="white"
          transform="translate(4 0.830078)"
        />
      </clipPath>
    </defs>
  </svg>
  <svg
    v-else-if="name === 'time'"
    :width="width ? width : 58"
    :height="height ? height : 59"
    viewBox="0 0 58 59"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <g clip-path="url(#clip0_1_565)" filter="url(#filter0_d_1_565)">
      <rect x="4" y="0.830078" width="50" height="50" rx="19" fill="#F03E3D" />
      <path
        d="M34.5714 20.2586H35.4286C35.5893 20.2586 35.7143 20.1336 35.7143 19.9729V19.4015C35.7143 19.2408 35.5893 19.1158 35.4286 19.1158H22.2857C22.125 19.1158 22 19.2408 22 19.4015V19.9729C22 20.1336 22.125 20.2586 22.2857 20.2586H23.1429C23.1429 23.5622 24.7232 25.9551 26.4732 27.1158C24.7232 28.2765 23.1429 30.6694 23.1429 33.9729H22.2857C22.125 33.9729 22 34.0979 22 34.2586V34.8301C22 34.9908 22.125 35.1158 22.2857 35.1158H35.4286C35.5893 35.1158 35.7143 34.9908 35.7143 34.8301V34.2586C35.7143 34.0979 35.5893 33.9729 35.4286 33.9729H34.5714C34.5714 30.6694 32.9911 28.2765 31.2411 27.1158C32.9911 25.9551 34.5714 23.5622 34.5714 20.2586ZM33.4286 20.2586C33.4286 21.5622 33.1339 22.714 32.6696 23.6872H25.0446C24.5804 22.714 24.2857 21.5622 24.2857 20.2586H33.4286ZM32.9196 31.1158H24.7946C25.4554 29.3926 26.6429 28.1694 27.8304 27.6872H29.8839C31.0714 28.1694 32.2589 29.3926 32.9196 31.1158Z"
        fill="white"
      />
    </g>
    <defs>
      <filter
        id="filter0_d_1_565"
        x="0"
        y="0.830078"
        width="58"
        height="58"
        filterUnits="userSpaceOnUse"
        color-interpolation-filters="sRGB"
      >
        <feFlood flood-opacity="0" result="BackgroundImageFix" />
        <feColorMatrix
          in="SourceAlpha"
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
          result="hardAlpha"
        />
        <feOffset dy="4" />
        <feGaussianBlur stdDeviation="2" />
        <feColorMatrix
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
        />
        <feBlend
          mode="normal"
          in2="BackgroundImageFix"
          result="effect1_dropShadow_1_565"
        />
        <feBlend
          mode="normal"
          in="SourceGraphic"
          in2="effect1_dropShadow_1_565"
          result="shape"
        />
      </filter>
      <clipPath id="clip0_1_565">
        <rect
          width="50"
          height="50"
          fill="white"
          transform="translate(4 0.830078)"
        />
      </clipPath>
    </defs>
  </svg>
</template>

<script>
export default {
  props: {
    name: String,
    width: Number,
    height: Number,
    fill: String,
  },
};
</script>

<style>
</style>