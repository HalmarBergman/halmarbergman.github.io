<template>
  <v-app id="app">
    <v-main>
      <div class="container">
        <div class="background">
          <div class="navbar">
            <img class="bitpic" src="@/assets/icons/bitpic.svg" />
            <h1 @click="readme()" class="navlinks" href="#">Profile</h1>
            <h1 @click="portfolio()" class="navlinks" href="#">Portfolio</h1>
            <h1 @click="socials()" class="navlinks" href="#">Socials</h1>
          </div>
          <div @click="trash()" class="iconlink trash">
            <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 48 48">
              <path
                d="M32.391,18.943v20.92H29.4V18.943H20.437v20.92H17.449V18.943H7.2A76.19,76.19,0,0,0,9.572,43.067a4.483,4.483,0,0,0,3.593,3.28,71.306,71.306,0,0,0,11.756.987,71.338,71.338,0,0,0,11.759-.987,4.486,4.486,0,0,0,3.593-3.28,76.355,76.355,0,0,0,2.376-24.125ZM44.346,8.483H33.886V6.989A2.987,2.987,0,0,0,30.9,4H18.944a2.991,2.991,0,0,0-2.989,2.989V8.483H5.5A1.494,1.494,0,0,0,4,9.977V14.46a1.494,1.494,0,0,0,1.5,1.494H44.346A1.493,1.493,0,0,0,45.84,14.46V9.977A1.493,1.493,0,0,0,44.346,8.483Z"
              />
            </svg>
            <div class="label">Trash</div>
          </div>
          <div @click="readme()" class="iconlink readme">
            <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="41" height="41" viewBox="0 0 41 41">
              <path
                d="M39.813,38.326c-2.494-11.664-17.671-7.219-11.981-16,3.339-5.372,3.936-9.987,1.772-13.721a8.71,8.71,0,0,0-15.367,0c-2.163,3.734-1.567,8.349,1.786,13.741,5.664,8.734-9.523,4.32-12.016,15.977a1.281,1.281,0,0,0,.886,1.5c.181.054,4.581,1.328,17.023,1.335h0c12.442-.008,16.829-1.281,17.01-1.335A1.281,1.281,0,0,0,39.813,38.326Z"
              />
            </svg>
            <div class="label">Read Me</div>
          </div>
          <div @click="portfolio()" class="iconlink portfolio">
            <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="41" height="41" viewBox="0 0 41 41">
              <path
                d="M37.876,17.531H15.457a2.989,2.989,0,0,0-2.721,2.225C12.4,21.086,8.943,34.313,8.8,34.743A1.958,1.958,0,0,1,6.663,36.11,1.557,1.557,0,0,1,5.43,34.1c.311-1.189,3.592-13.642,3.93-14.97a5.149,5.149,0,0,1,5.2-4.156H35.313V12.406a2.562,2.562,0,0,0-2.562-2.563H16.184l-1.8-2.7A2.562,2.562,0,0,0,12.251,6H4.563A2.563,2.563,0,0,0,2,8.563V37.046a2.562,2.562,0,0,0,2.239,2.542,104.783,104.783,0,0,0,28.836,0,2.7,2.7,0,0,0,2.4-1.878L40.339,20.8A2.563,2.563,0,0,0,37.876,17.531Z"
              />
            </svg>
            <div class="label">Portfolio</div>
          </div>
          <div @click="socials()" class="iconlink socials">
            <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="42" height="42" viewBox="0 0 42 42">
              <path
                d="M40.305,14.2a6.614,6.614,0,0,0-5.743-5.485,103.857,103.857,0,0,0-23.914,0A6.614,6.614,0,0,0,4.9,14.2a62.451,62.451,0,0,0,0,20.818A6.614,6.614,0,0,0,10.648,40.5a103.364,103.364,0,0,0,23.914,0,6.614,6.614,0,0,0,5.743-5.485A62.451,62.451,0,0,0,40.305,14.2ZM30.384,25.621a50.868,50.868,0,0,1-12.49,7.628,1.38,1.38,0,0,1-1.9-1.157,91.3,91.3,0,0,1,0-15.027,1.381,1.381,0,0,1,1.9-1.158,50.867,50.867,0,0,1,12.49,7.628A1.383,1.383,0,0,1,30.384,25.621Z"
              />
            </svg>
            <div class="label">Social Media</div>
          </div>
          <ReadmeModal v-if="appstate === 'readme'" />
          <PortfolioModal v-if="appstate === 'portfolio'" />
          <SocialsModal v-if="appstate === 'socials'" />
          <TrashModal v-if="appstate === 'trash'" />
        </div>
      </div>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ReadmeModal from "./views/ReadmeModal.vue";
import PortfolioModal from "./views/PortfolioModal.vue";
import SocialsModal from "./views/SocialsModal.vue";
import TrashModal from "./views/TrashModal.vue";
import Scriptie from "./components/Scriptie.vue";
import "@/assets/css/main.scss";

@Component({
  components: {
    ReadmeModal,
    PortfolioModal,
    SocialsModal,
    TrashModal,
    Scriptie,
  },
})
export default class App extends Vue {
  appstate = "desktop";

  trash() {
    this.appstate = "trash";
  }
  readme() {
    this.appstate = "readme";
  }
  portfolio() {
    this.appstate = "portfolio";
  }
  socials() {
    this.appstate = "socials";
  }
}
</script>
