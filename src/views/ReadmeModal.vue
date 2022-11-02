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
          <h2 class="contentsubtitle intext">Profile</h2>
          <p class="contenttext">
            I currently work as a UI/UX Designer and Front-End Developer at Figrs. Besides that, I am also getting my masters in information
            studies at the university of Amsterdam.
          </p>

          <h2 class="contentsubtitle intext">Experience</h2>
          <h2 class="contentsubtitle workplace">Figrs</h2>
          <h2 class="contentsubtitle function">UI/UX Designer & Front-End Developer | 2022 - today</h2>
          <p class="contenttext">
            As a UI/UX Designer at Figrs in Apeldoorn, I am able to experience experience in the design and development of complext software
            applications intended for clients. Here I frequently work with:
            <ul class="contentlist">
              <li class="contentlistitem">Adobe XD</li>
              <li class="contentlistitem">HTML</li>
              <li class="contentlistitem">CSS</li>
              <li class="contentlistitem">JavaScript</li>
              <li class="contentlistitem">Vue.js</li>
              <li class="contentlistitem">Node.js</li>
              <li class="contentlistitem">ETL</li>
              <li class="contentlistitem">Azure Data Fundamentals</li>
            </ul>
          </p>

          <h2 class="contentsubtitle workplace">Lead Healthcare</h2>
          <h2 class="contentsubtitle function">Technical Support Agent | 2021 - 2022</h2>
          <p class="contenttext">
            As a technical support agent at Lead Healthcare, I was able to actively contribute in the testenvoortoegang.nl policy, which enabled thousands of people to go out during the covid pandemic. I frequently worked with: 
            <ul class="contentlist">
              <li class="contentlistitem">Jira</li>
              <li class="contentlistitem">the Development Team</li>
            </ul>
          </p>

          <h2 class="contentsubtitle workplace">Royal Huisman BV</h2>
          <h2 class="contentsubtitle function">IT-Consultant | 2018 - 2019</h2>
          <p class="contenttext">
            At Royal Huisman, I was asked to help with the organization and digitalization of the large amount of work-tools in the company. Setting up a system that tracks usage of the equipment.
          </p>

          <h2 class="contentsubtitle workplace">Albert Heijn Havelte</h2>
          <h2 class="contentsubtitle function">Shiftleader | 2016 - 2019</h2>
          <p class="contenttext">
            As a shiftleader at the Albert Heijn supermarket, I was responsible for filling crews of 20+ people. I gained experience in:
            <ul class="contentlist">
              <li class="contentlistitem">Leadership</li>
              <li class="contentlistitem">Teamwork</li>
              <li class="contentlistitem">Proposing new best-practice processes</li>
            </ul>
          </p>

          <h2 class="contentsubtitle intext">Education</h2>
          <h2 class="contentsubtitle workplace">Bachelor</h2>
          <h2 class="contentsubtitle function">Information Sciences</h2>
          <p class="contenttext">
            Utrecht University <br/>
            2019 - 2022
          </p>

          <h2 class="contentsubtitle workplace">Minor</h2>
          <h2 class="contentsubtitle function">Innovation Sciences</h2>
          <p class="contenttext">
            Utrecht University <br/>
            2021 - 2022
          </p>

          <h2 class="contentsubtitle workplace">Master</h2>
          <h2 class="contentsubtitle function">Information Studies</h2>
          <p class="contenttext">
            Univeristy of Amsterdam <br/>
            2022 - today
          </p>

          <h2 class="contentsubtitle intext">Certificates</h2>
          <h2 class="contentsubtitle workplace">Microsoft</h2>
          <h2 class="contentsubtitle function">Azure Data Fundamentals</h2>
          <p class="contenttext">
            DP-900 <br/>
            October 2022
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
