<template>
  <div id="portfoliomodal">
    <div class="mainscreen">
      <div class="modalbg"></div>
      <div class="modal" v-if="portfoliostate === 'portfolio'">
        <div class="modalheader">
          <h1 class="modaltitle">Portfolio</h1>
          <div class="modalclose">
            <img class="closeicon" src="@/assets/icons/close.svg" />
          </div>
        </div>
        <div class="modalscrolling"></div>
        <div class="modalcontent portfolio">
          <div @click="scriptiedetails()" class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">thesis_project</p>
          </div>
          <div @click="project1details()" class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">ABC_Construction</p>
          </div>
        </div>
      </div>

      <Scriptie v-if="portfoliostate === 'scriptiedetails'" />
      <ABC_Construction v-if="portfoliostate === 'ABC_Construction'" />
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Scriptie from "@/components/Scriptie.vue";
import ABC_Construction from "@/components/ABC_construction.vue";
import "@/assets/css/main.scss";
import "@/assets/css/modal.scss";

@Component({
  components: {
    ABC_Construction,
    Scriptie,
  },
})
export default class PortfolioModal extends Vue {
  portfoliostate = "portfolio";

  scriptiedetails() {
    this.portfoliostate = "scriptiedetails";
  }
  project1details() {
    this.portfoliostate = "ABC_Construction";
  }

}
</script>
