<template>
  <div class="github-state">
    <div class="github-logo">
      <app-icon icon="github" color="#ffffff" size="32" />
      <div>
        <span style="font-weight: bold; margin-bottom: 3px">Github</span>
        <span style="font-size: 0.8rem">资料卡</span>
      </div>
    </div>
    <div class="github-star">
      <i class="el-icon-star-off" />
      <span>2</span>
    </div>
    <div class="github-cat">
      <svg
        aria-hidden="true"
        width="106"
        height="60"
        viewBox="0 0 106 60"
        fill="none"
        stroke-width="3"
        stroke-linecap="round"
        stroke-linejoin="round"
        xmlns="http://www.w3.org/2000/svg"
      >
        <g>
          <path
            stroke="#da3633"
            d="M37.5 58.5V57.5C37.5 49.768 43.768 43.5 51.5 43.5V43.5C59.232 43.5 65.5 49.768 65.5 57.5V58.5"
          ></path>
        </g>
        <g>
          <path
            stroke="#f0883e"
            d="M104.07 58.5C103.401 55.092 97.7635 54.3869 95.5375 57.489C97.4039 54.6411 99.7685 48.8845 94.6889 46.6592C89.4817 44.378 86.1428 50.1604 85.3786 54.1158C85.9519 50.4768 83.7226 43.294 78.219 44.6737C72.7154 46.0534 72.7793 51.3754 74.4992 55.489C74.169 54.7601 72.4917 53.3567 70.5 52.8196"
          ></path>
        </g>
        <g>
          <path
            stroke="#8957e5"
            d="M5.51109 58.5V52.5C5.51109 41.4543 14.4654 32.5 25.5111 32.5C31.4845 32.5 36.8464 35.1188 40.5111 39.2709C40.7212 39.5089 40.9258 39.7521 41.1245 40"
          ></path>
          <path
            stroke="#8957e5"
            d="M27.511 49.5C29.6777 49.5 28.911 49.5 32.511 49.5"
          ></path>
          <path
            stroke="#8957e5"
            d="M27.511 56.5C29.6776 56.5 26.911 56.5 30.511 56.5"
          ></path>
        </g>
        <g>
          <circle stroke="#3fb950" cx="5.5" cy="12.5" r="4"></circle>
          <circle stroke="#3fb950" cx="18.5" cy="5.5" r="4"></circle>
          <path stroke="#3fb950" d="M18.5 9.5L18.5 27.5"></path>
          <path
            stroke="#3fb950"
            d="M18.5 23.5C6 23.5 5.5 23.6064 5.5 16.5"
          ></path>
        </g>
        <g>
          <path
            stroke="#388bfd"
            d="M45.3697 34.2658C41.8877 32.1376 39.7113 28.6222 39.7113 23.2283C39.7113 20.3101 40.3483 17.7986 41.4845 15.6968C40.3605 11.9182 39.662 6.85125 40.7522 5.23168C42.5699 2.53117 49.3177 4.6027 52.1188 8.24095C53.831 7.85521 55.6556 7.66186 57.5491 7.66186C59.3929 7.66186 61.1713 7.84519 62.8442 8.21095C65.6593 4.59134 72.375 2.5386 74.1877 5.23168C75.2599 6.82461 74.6019 11.7525 73.5105 15.5094C74.7112 17.6488 75.3869 20.2229 75.3869 23.2283C75.3869 28.6222 73.2105 32.1376 69.7285 34.2658C70.8603 35.5363 72.6057 38.3556 73.3076 40"
          ></path>
          <path stroke="#388bfd" d="M49.0747 19.8242V22.4999"></path>
          <path
            stroke="#388bfd"
            d="M54.0991 28C54.6651 29.0893 55.7863 30.0812 57.9929 30.0812C59.0642 30.0812 59.8797 29.8461 60.5 29.4788"
          ></path>
          <path stroke="#388bfd" d="M66.9126 19.8242V22.4999"></path>
          <path stroke="#388bfd" d="M33.2533 20.0237L39.0723 22.1767"></path>
          <path stroke="#388bfd" d="M39.1369 25.0058L33.0935 27.3212"></path>
          <path stroke="#388bfd" d="M81.8442 19.022L76.0252 21.1751"></path>
          <path stroke="#388bfd" d="M75.961 24.0041L82.0045 26.3196"></path>
        </g>
      </svg>
    </div>
    <a class="github-link" target="_blank" href="https://github.com/someGenki">
      github.com/someGenki
    </a>
  </div>
</template>

<script>
// 猫猫图标来自Github/profile页面 若有侵权 马上删除
export default {
  name: 'GithubState',
}
</script>

<style lang="scss" scoped>
$theme-color: #161b22;
$card-height: 160px;
.github-state {
  height: $card-height;
  padding: 10px;
  border-radius: 8px;
  background-color: $theme-color;
  position: relative;
}
.github-logo {
  display: flex;
  align-items: center;
  > div {
    display: inline-flex;
    flex-direction: column;
    color: white;
    margin-left: 10px;
  }
}
.github-cat {
  position: absolute;
  right: 6px;
  bottom: 0;
}
.github-link {
  position: absolute;
  left: 8px;
  bottom: 6px;
  color: #eee;
  font-size: 0.8rem;
  &:hover {
    border-bottom: 1px solid #eee;
  }
}
.github-star {
  position: absolute;
  top: 10px;
  right: 20px;
  color: #eee;
  font-size: 1.2rem;
  span {
    margin-left: 6px;
  }
}
</style>
