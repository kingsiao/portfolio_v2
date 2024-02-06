<template>
  <div class="desc-container">
    <div class="desc-container__item">
      <p class="name-text">King Solomon Siao</p>
      <p class="job-text">Software Engineer at <span class="company-text">Yondu Inc.</span></p>
      <div>
        <a href="https://www.facebook.com/profile.php?id=100008348959213"
          ><FacebookIcon class="icon"
        /></a>
        <a href="https://github.com/kingsiao"><GithubIcon class="icon" /></a>
        <a href="https://www.linkedin.com/in/king-solomon-siao-678370176/"
          ><LinkedInIcon class="icon"
        /></a>
        <a href="https://www.instagram.com/kingsiao/"><InstagramIcon class="icon" /></a>
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
</style>
