<template>
  <div class="desc-container">
    <div class="desc-container__item">
      <p class="name-text">King Solomon Siao</p>
      <p class="job-text">Software Engineer at <span class="company-text">Yondu Inc.</span></p>
      <div>
        <a href="#"><FacebookIcon class="icon" /></a>
        <a href="#"><GithubIcon class="icon" /></a>
        <a href="#"><LinkedInIcon class="icon" /></a>
        <a href="#"><InstagramIcon class="icon" /></a>
      </div>
    </div>
  </div>
</template>

<script setup>
import LinkedInIcon from '../assets/icons/linkedin.vue'
import FacebookIcon from '../assets/icons/facebook.vue'
import InstagramIcon from '../assets/icons/instagram-alt.vue'
import GithubIcon from '../assets/icons/github.vue'
</script>

<style scoped lang="scss">
.desc-container {
  // border: 1px solid aqua;
  width: 50vw;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  &__item {
    position: fixed;
    & div {
      margin-left: -5px;
      margin-top: 5px;
    }
    & .name-text {
      color: white;
      font-size: 45px;
    }
    & .job-text {
      color: #5ae0d3;
      font-size: 25px;
      padding-bottom: 5px;
      & .company-text {
        font-size: 25px;
        color: white;
      }
    }
  }
}

@media (min-width: 250px) and (max-width: 870px) {
  .desc-container {
    width: 100vw !important;
    padding: 20px;
    &__item {
      position: relative;
      width: auto;
      margin: 0;
      & .icon {
        width: 30px;
        height: 30px;
      }
      & .name-text {
        font-size: 30px;
      }
      & .job-text {
        font-size: 18px;
        padding-bottom: 5px;
        & .company-text {
          font-size: 18px;
        }
      }
    }
  }
}

// @media (min-width: 401px) and (max-width: 870px) {
//   .desc-container {
//     width: 100vw !important;
//     display: flex;
//     flex-direction: row !important;
//     &__item {
//       position: absolute;
//     }
//   }
// }
</style>
