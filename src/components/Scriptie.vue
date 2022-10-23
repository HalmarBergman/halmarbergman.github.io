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
          <img class="detailsimage" src="@/assets/icons/phishing.svg" />
          <div class="tags">
            <div class="tag">Academic Writing</div>
            <div class="tag">UI/UX Designing</div>
          </div>
          <h1 class="contenttitle">
            The Influence of Several of Cialdini’s Persuasive Principles on the Effectiveness of Several Categories of Phishing Attacks.
          </h1>
          <div class="contentsubtitles">
            <h2 class="contentsubtitle">
              Persuasive Principles, Phishing Attack, User Persuasiveness, Certainty Scores, Cybercriminals, Phishing.
            </h2>
          </div>
          <p class="contenttext">
            Phishing Attacks are criminal mechanisms employing both social engineering and technical subterfuge to steal consumers’ personal
            identity data and financial account credentials. Persuasive Principles, which are social engineering techniques used to
            influence people's decision making, are frequently used to strengthen such criminal enterprises. The current study aims to
            retrieve more knowledge about these concepts by looking at the relation they have with each other. First of all, it investigates
            the effect Persuasive Principles have on the succession rate of Phishing Attacks. Second, it captures a user's level of
            certainty for each of the Phishing Attacks and the difference as a result of the implementation of Persuasive Principles, and
            determines a Phishing Attack ranking, from this level of certainty. <br />
            <br />
          </p>
          <p class="contenttext">
            As the world is becoming ever more digital (Leeflang et al., 2014), we are actively and continuously transforming from an analog
            world to a world where almost everything in daily life has some aspects of it in a digital form. Digital technologies have
            advanced more rapidly than any other innovation in our history - reaching around 50% of the developing world’s population in
            only two decades and transforming entire societies (United Nations, 2020). In these two decades, as a result of the
            digitalization of business processes, social interactions and information, basic personal information like names, email
            addresses, financial information, and even sometimes home addresses have eventually ended up online (Mai, 2016). Throughout the
            last decades, technology has advanced substantially and has spread into people’s every-day lives (Kim, 2015). <br /><br />
            These digitalizations bring tremendous amounts of benefits along with them in our daily lives. We now have the ability to work
            from home and communicate with anyone, anywhere by email with just the click of a button. We can scan, select and order
            groceries from our couch, while quickly checking our bank statements in a mobile application. We can meet up with our friends
            through our screens, send them messages, pictures, and videos to share our daily ventures. We have access to the most relevant
            and important news articles within seconds, while also having the capability to research the validity of these articles with a
            simple ‘google’ when we wish too. We can search for old friends on Facebook to see what they are up to. We can simply enjoy a
            nice afternoon on the couch while watching almost all series or movies that I want to watch. We live in a world that has changed
            beyond recognition in the last few decades, where it is almost possible to live your entire life online or through technology
            (Lilley, 2002). <br />
            <br />
            As with almost all innovations in history, innovations almost always come with risks. The digitalization... <br />
            <br /><br />
            <br />
          </p>
          <!-- TODO: It downloads as html for some reason -->
          <a href="@/assets/images/bachelor_thesis_halmar.pdf" class="downloadscriptie" download="BachelorThesis_Halmar"
            >Download Entire Thesis</a
          >
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
export default class Scriptie extends Vue {}
</script>
