<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import SelfIntroComponent from "./components/SelfIntroComponent.vue";
import NewsletterComponent from "./components/NewsletterComponent.vue";
import SkillsComponent from "./components/SkillsComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  data() {
    return {
      websiteName: "My Portfolio",
    };
  },
  components: {
    HeaderComponent,
    SelfIntroComponent,
    NewsletterComponent,
    SkillsComponent,
    FooterComponent,
  },
};
</script>

<template>
  <HeaderComponent v-bind:websiteName="websiteName"></HeaderComponent>
  <SelfIntroComponent></SelfIntroComponent>

  <div class="row align-items-md-stretch">
    <div class="col-md-6">
      <NewsletterComponent></NewsletterComponent>
    </div>

    <div class="col-md-6">
      <SkillsComponent></SkillsComponent>
    </div>
  </div>
      <FooterComponent v-bind:websiteName="websiteName"></FooterComponent>
</template>

<style></style>
