<template>
  <div id="trashmodal">
    <div class="mainscreen">
      <div class="modalbg"></div>
      <div class="modal">
        <div class="modalheader">
          <h1 class="modaltitle">Trash</h1>
          <div @click="empty()" class="emptytrash">Empty</div>
          <div class="modalclose">
            <img class="closeicon" src="@/assets/icons/close.svg" />
          </div>
        </div>
        <div class="modalscrolling"></div>
        <div class="modalcontent trash" v-if="trashstate === 'show'">
          <div class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">WordPress</p>
          </div>
          <div class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">Elementor</p>
          </div>
          <div class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">Lorem</p>
          </div>
          <div class="file">
            <svg class="file" xmlns="http://www.w3.org/2000/svg" width="122" height="122" viewBox="0 0 122 122">
              <path
                d="M96.922,6C78.993.89,34.9.513,10.509,5.919A5.738,5.738,0,0,0,6,11.489v95.061a5.739,5.739,0,0,0,4.5,5.57c.728.16,18.005,3.936,44.941,3.936.938,0,4.02.013,7.648-.245,10.757-.765,37.967-27.184,37.967-37.777V11.489A5.7,5.7,0,0,0,96.922,6ZM82.077,81.834H70.67a4.481,4.481,0,0,0-3.834,3.8V97.044a7.873,7.873,0,0,1-7.6,7.6V85.637c0-5.863,5.572-11.445,11.439-11.445H89.682A7.909,7.909,0,0,1,82.077,81.834Z"
              />
            </svg>
            <p class="filename">Lorem</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import "@/assets/css/modal.scss";

@Component({
  components: {},
})
export default class TrashModal extends Vue {
  trashstate = "show";

  empty() {
    this.trashstate = "hide";
  }
}
</script>
