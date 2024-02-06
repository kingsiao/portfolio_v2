<template>
  <div class="about-container">
    <div class="about-container__item">
      <p>
        💡 Armed with a passion for innovation and a knack for problem-solving I thrive in the
        dynamic world of software development. My journey involves crafting solutions that
        seamlessly blend cutting-edge technology with user-centric design.
      </p>

      <p>
        🌐 Specializing in a diverse tech stack, I'm fluent in the languages of
        <span class="highlight-text">HTML</span>, <span class="highlight-text">CSS</span>, and
        <span class="highlight-text">Javascript</span>. My toolkit extends to powerful frameworks
        like <span class="highlight-text">ReactJS</span>, <span class="highlight-text">VueJS</span>,
        and the versatility of <span class="highlight-text">NextJS</span> and
        <span class="highlight-text">NuxtJS</span>. On the server side, I harness the capabilities
        of <span class="highlight-text">ExpressJS</span> and
        <span class="highlight-text">NodeJS</span>, ensuring a robust foundation for every project.
      </p>

      <p>
        🛠️ With a keen eye for detail, I delve into the intricacies of software architecture,
        creating scalable and efficient solutions. <span class="highlight-text">MongoDB</span> is my
        playground for data management, where I sculpt databases that not only store information but
        tell compelling stories.
      </p>
    </div>

    <div class="border-line"></div>

    <div class="about-container__item">
      <h1 class="headline">Projects</h1>
      <div class="project-table-head">
        <span>Year</span>
        <span>Project</span>
        <span>Built with</span>
        <span>Link</span>
      </div>
      <div class="project-table-data">
        <div>
          <p>2023</p>
        </div>

        <div>
          <p>Healthnow</p>
        </div>

        <div>
          <p>React.js</p>
          <p>Next.js</p>
          <p>GraphQL</p>
          <p>Node.js</p>
          <p>MongoDB</p>
          <p>Insomnia</p>
        </div>

        <div>
          <a href="#">
            <LinkIcon class="icon" />
          </a>
        </div>
      </div>

      <div class="project-table-data">
        <div>
          <p>2023</p>
        </div>

        <div>
          <p>LoadUp</p>
        </div>

        <div>
          <p>Vue.js</p>
          <p>BootstrapVue</p>
          <p>Nuxt.js</p>
          <p>Node.js</p>
        </div>

        <div>
          <a href="#">
            <LinkIcon class="icon" />
          </a>
        </div>
      </div>
    </div>

    <div class="border-line"></div>

    <div class="about-container__item">
      <h1 class="headline">Get In Touch</h1>

      <div class="personal-details-container">
        <div>
          <div>
            <LocationIcon class="icon" />
          </div>

          <div>
            <PhoneIcon class="icon" />
          </div>

          <div>
            <EnvelopeIcon class="icon" />
          </div>
        </div>
        <div>
          <span
            >Manila, <br />
            Philippines</span
          >
          <span>kingsolomonsiao <br />@gmail.com</span>
          <span>09973900735</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import LinkIcon from '../assets/icons/external-link-alt.vue'
import LocationIcon from '../assets/icons/map-marker-alt.vue'
import PhoneIcon from '../assets/icons/phone.vue'
import EnvelopeIcon from '../assets/icons/envelope.vue'
</script>

<style scoped lang="scss">
.highlight-text {
  color: #5ae0d3;
}
.about-container {
  // border: 1px solid aqua;
  width: 50vw;
  padding: 5%;
  margin-bottom: 30px;
  &__item {
    // border: 1px solid aqua;
    p {
      margin: 20px 0;
      font-size: 18px;
    }
    & .headline {
      color: #fff;
      text-align: center;
      padding: 25px 0;
      font-size: 40px;
      font-weight: 600;
    }
    & .project-table-head {
      display: flex;
      justify-content: space-between;
      font-size: 20px;
      color: #fff;
      gap: 0 !important;
      & span:nth-child(1) {
        width: 15%;
        padding: 0 5px;
      }
      & span:nth-child(2) {
        width: 25%;
        padding: 0 5px;
      }
      & span:nth-child(3) {
        width: 50%;
        padding: 0 5px;
      }
      & span:nth-child(4) {
        width: 10%;
        padding: 0 5px;
      }
    }
    & .project-table-data {
      display: flex;
      justify-content: space-between;
      & div:nth-child(1) {
        width: 15%;
        padding: 0 5px;
      }
      & div:nth-child(2) {
        width: 25%;
        color: #fff;
        padding: 0 5px;
      }
      & div:nth-child(3) {
        display: flex;
        flex-wrap: wrap;
        width: 50%;
        gap: 0 5px !important;
        padding: 5px 5px 0 5px;
        p {
          padding: 10px 5px;
          border-radius: 10px;
          color: #5ae0d3;
          background-color: #132d43;
          margin: 5px 2px !important ;
        }
      }
      & div:nth-child(4) {
        width: 10%;
        padding: 0 5px;
        padding-top: 20px;
        padding-left: 7px;
      }
    }
    & .personal-details-container {
      & div {
        display: flex;
        justify-content: center;
        align-items: center;
        & div {
          background-color: #132d43;
          border-radius: 50% !important;
          padding: 30px;
          margin: auto;
        }
        & span {
          width: 33%;
          display: flex;
          justify-content: space-around;
          margin-top: 10px;
          font-weight: 600;
          font-size: 18px;
          color: #5ae0d3;
        }
        & span:nth-child(1),
        span:nth-child(2) {
          text-align: center;
          display: flex;
        }
      }
    }
  }
  & .border-line {
    border: 1px solid #707070;
    margin-top: 85px;
  }
}

@media (min-width: 250px) and (max-width: 870px) {
  .icon {
    height: 20px;
    width: 20px;
  }
  .about-container {
    width: 100vw !important;
    &__item {
      p {
        margin: 15px 5px;
        font-size: 15px;
      }
      & .headline {
        font-size: 30px;
        font-weight: 600;
      }
      & .project-table-head {
        font-size: 15px;
        & span:nth-child(1) {
          margin-left: 3px;
        }
        & span:nth-child(2) {
          width: 25%;
          margin-left: 3px;
        }
        & span:nth-child(3) {
          width: 50%;
        }
      }
      & .project-table-data {
        & div:nth-child(2) {
          width: 25%;
        }
        & div:nth-child(3) {
          width: 50%;
        }
        p {
          font-size: 12px;
        }
      }
      & .personal-details-container {
        & div {
          padding: 10px;
          & span {
            font-size: 12px;
          }
          & span:nth-child(1) {
            text-align: center;
            display: flex;
          }
          & span:nth-child(2) {
            text-align: center;
            display: flex;
          }
        }
      }
    }
  }
}
</style>
