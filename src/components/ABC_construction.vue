<template>
  <div id="portfoliomodal">
    <div class="mainscreen">
      <div class="modalbg"></div>
      <div class="modal scriptie">
        <div class="modalheader">
          <h1 class="modaltitle">Portfolio Details</h1>
          <div class="modalclose">
            <img class="closeicon" src="@/assets/icons/close.svg" />
          </div>
        </div>
        <div class="modalscrolling"></div>
        <div class="modalcontent">
          <div class="contentimages">
            <img class="contentimage" src="@/assets/images/ABC1.png" />
            <img class="contentimage" src="@/assets/images/ABC2.png" />
            <img class="contentimage" src="@/assets/images/ABC3.png" />
            <img class="contentimage" src="@/assets/images/ABC4.png" />
            <img class="contentimage" src="@/assets/images/ABC5.png" />
            <img class="contentimage" src="@/assets/images/ABC6.png" />
            <img class="contentimage" src="@/assets/images/ABC7.png" />
          </div>
          <br />
          <br /><br />
          <br />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import "@/assets/css/main.scss";
import "@/assets/css/modal.scss";

@Component({
  components: {},
})
export default class ABC_Construction extends Vue {}
</script>
