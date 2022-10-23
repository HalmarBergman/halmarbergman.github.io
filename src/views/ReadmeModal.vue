<template>
  <div id="readmodal">
    <div class="mainscreen">
      <div class="modalbg"></div>
      <div class="modal">
        <div class="modalheader">
          <h1 class="modaltitle">Read Me</h1>
          <div class="modalclose">
            <img class="closeicon" src="@/assets/icons/close.svg" />
          </div>
        </div>
        <div class="modalscrolling"></div>
        <div class="modalcontent">
          <img class="bitpic large" src="@/assets/icons/bitpic.svg" />
          <h1 class="contenttitle">Halmar Henrik Bjarne Bergman</h1>
          <div class="contentsubtitles">
            <h2 class="contentsubtitle">UI/UX Designer</h2>
            <h2 class="contentsubtitle">Frontend Developer</h2>
          </div>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt,
          </p>

          <h2 class="contentsubtitle intext">Education</h2>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt, <br />
            <br />
          </p>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt,
          </p>

          <h2 class="contentsubtitle intext">Experience</h2>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt, <br />
            <br />
          </p>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt,
          </p>
          <h2 class="contentsubtitle intext">Socials</h2>
          <p class="contenttext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula,
            eget aliquam nisl nunc eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc
            eget nisl. Sed tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed
            tincidunt, nisl eget ultricies tincidunt, nisl elit aliquam ligula, eget aliquam nisl nunc eget nisl. Sed tincidunt,
          </p>
          <br /><br /><br /><br /><br /><br />
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
export default class ReadmeModal extends Vue {}
</script>
