<template>
  <div class="home">
      <!-- <transition name="slide-y-transition" appear> -->
        <paw class="paw mb-5"></paw>
      <!-- </transition> -->
      <transition name="slide-y-reverse-transition" appear>
        <img id="logotype" src="../assets/m_b_type.svg" alt="Maxime Barthelme Logotype" class="mb-4">
      </transition>
      <transition name="slide-y-reverse-transition" appear>
        <div class="bio mb-4">
          <p class="font-regular title">Photographer, Videographer, Drone Pilot & Polar Guide</p>
        </div>
      </transition>
    <div class="links-container">
        <a :href="link.url" class="pa-1 headline font-regular" target="_blank" v-for="(link, index) in links" :key="link.url">
          <transition name="slide-y-reverse-transition" appear>
              <v-icon large class="pa-1 mt-1" :style="{ transitionDelay: 1100 + (index * 100) + 'ms'}">{{link.icon}}</v-icon> 
          </transition>
        </a>
    </div>
  </div>
</template>

<script>
import Paw from '../components/Paw'

export default {
  name: 'home',
  components: {
    Paw
  },
  data () {
    return {
      links: [
        {
          icon: 'mdi-instagram',
          url: 'https://www.instagram.com/maximebarthelme/'
        },
        {
          icon: 'mdi-facebook',
          url: 'https://www.facebook.com/MaximeBarthelme/'
        },
        {
          icon: 'mdi-email-outline',
          url: 'mailto:barthelme.maxime@gmail.com'
        }
      ]
    }
  }
}
</script>

<style lang="postcss" scoped>
.home {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.link-container {
  display: flex;
  flex-direction: row;
  align-items: center;
}


#logotype {
  width: 381px;
  transition-delay: 900ms;
}

.bio {
  transition-delay: 1000ms;
}

@media (width <= 500px) {
  .paw {
    width: 180px;
  }

  #logotype {
    width: 300px;
  }

  .bio {
    width: 300px;
    font-size: 15px!important;
    text-align: center;
  }
}

</style>

