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
  <svg
    v-else-if="name === 'check'"
    :width="width ? width : 16"
    :height="height ? height : 13"
    viewBox="0 0 16 13"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M15.7657 0.540581C15.4533 0.221499 14.9468 0.221499 14.6343 0.540581L5.04982 10.329L1.3657 6.56653C1.0533 6.24745 0.546796 6.24748 0.234328 6.56653C-0.0781093 6.88558 -0.0781093 7.40285 0.234328 7.72194L4.48414 12.0621C4.79645 12.3811 5.30332 12.3809 5.61551 12.0621L15.7657 1.69602C16.0781 1.37697 16.0781 0.859663 15.7657 0.540581Z"
      :fill="fill ? fill : 'white'"
    />
  </svg>
  <svg
    v-else-if="name === 'star-fill'"
    :width="width ? width : 19"
    :height="height ? height : 19"
    viewBox="0 0 19 19"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M18.2961 6.58663C18.2384 6.41682 18.1323 6.26761 17.9908 6.15742C17.8493 6.04723 17.6787 5.98089 17.4999 5.96658L12.2708 5.55107L10.008 0.542056C9.9359 0.380725 9.81869 0.243699 9.67047 0.147514C9.52225 0.0513295 9.34936 9.71158e-05 9.17266 1.37932e-07C8.99597 -9.684e-05 8.82302 0.0509458 8.6747 0.146968C8.52637 0.24299 8.40901 0.379887 8.33677 0.541138L6.07395 5.55107L0.844797 5.96658C0.669105 5.9805 0.501144 6.04474 0.361006 6.15161C0.220868 6.25849 0.114488 6.40348 0.0545932 6.56923C-0.00530196 6.73498 -0.0161763 6.91448 0.0232713 7.08625C0.062719 7.25802 0.150818 7.41479 0.277029 7.5378L4.14134 11.3049L2.77466 17.2229C2.73316 17.402 2.74646 17.5895 2.81283 17.761C2.8792 17.9324 2.99559 18.08 3.14687 18.1845C3.29816 18.2891 3.47737 18.3457 3.66124 18.3471C3.84511 18.3485 4.02516 18.2946 4.17803 18.1924L9.17237 14.8628L14.1667 18.1924C14.3229 18.2961 14.5072 18.3495 14.6947 18.3454C14.8822 18.3413 15.0639 18.2799 15.2155 18.1694C15.367 18.0589 15.4811 17.9047 15.5423 17.7274C15.6036 17.5502 15.6091 17.3584 15.5581 17.1779L13.8805 11.3076L18.0411 7.56348C18.3135 7.31766 18.4135 6.93426 18.2961 6.58663Z"
      :fill="fill ? fill : '#F3CD03'"
    />
  </svg>
  <svg
    v-else-if="name === 'star-outline'"
    :width="width ? width : 19"
    :height="height ? height : 19"
    viewBox="0 0 19 19"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M4.19767 11.3049L2.83099 17.2229C2.78867 17.4021 2.80138 17.5899 2.86745 17.7618C2.93352 17.9336 3.04988 18.0816 3.20135 18.1863C3.35281 18.291 3.53232 18.3476 3.71645 18.3487C3.90057 18.3498 4.08075 18.2953 4.23345 18.1924L9.22779 14.8629L14.2221 18.1924C14.3784 18.2962 14.5626 18.3496 14.7501 18.3454C14.9376 18.3413 15.1193 18.2799 15.2709 18.1694C15.4224 18.0589 15.5365 17.9047 15.5978 17.7274C15.659 17.5502 15.6645 17.3584 15.6136 17.178L13.9359 11.3077L18.0965 7.56351C18.2298 7.44353 18.3249 7.28712 18.3702 7.11362C18.4155 6.94012 18.409 6.75715 18.3514 6.58734C18.2938 6.41752 18.1877 6.26831 18.0463 6.15815C17.9048 6.04799 17.7341 5.98172 17.5554 5.96752L12.3262 5.5511L10.0634 0.542085C9.99123 0.380794 9.87394 0.243833 9.72567 0.147729C9.5774 0.0516259 9.40448 0.000488281 9.22779 0.000488281C9.05109 0.000488281 8.87817 0.0516259 8.7299 0.147729C8.58163 0.243833 8.46434 0.380794 8.39219 0.542085L6.12937 5.5511L0.900217 5.96661C0.724525 5.98053 0.556564 6.04477 0.416426 6.15164C0.276288 6.25852 0.169908 6.40351 0.110013 6.56926C0.050118 6.73501 0.0392436 6.91451 0.0786913 7.08628C0.118139 7.25805 0.206238 7.41482 0.332449 7.53783L4.19767 11.3049ZM6.81454 7.33696C6.97826 7.32406 7.1355 7.26735 7.26977 7.17278C7.40404 7.07821 7.51039 6.94927 7.57768 6.79946L9.22779 3.14795L10.8779 6.79946C10.9452 6.94927 11.0515 7.07821 11.1858 7.17278C11.3201 7.26735 11.4773 7.32406 11.641 7.33696L15.2843 7.62588L12.284 10.3262C12.0235 10.561 11.9199 10.9224 12.0153 11.26L13.1646 15.282L9.73777 12.9972C9.58736 12.8963 9.41031 12.8423 9.22916 12.8423C9.04801 12.8423 8.87097 12.8963 8.72055 12.9972L5.13967 15.3848L6.10277 11.215C6.13808 11.0617 6.13334 10.9018 6.08901 10.7508C6.04467 10.5998 5.96223 10.4627 5.84961 10.3528L3.06305 7.63597L6.81454 7.33696Z"
      :fill="fill ? fill : '#F3CD03'"
    />
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