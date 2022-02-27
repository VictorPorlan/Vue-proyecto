<template>
  <div class="about">
    <Header selected="About" />
    <div class="bodyAbout">
      <LongCard />
      <div class="group">
        <SmallCard
          title="LAND TRANSPORT"
          text="This website template has been designed by Free Website Templates for you, for free. You can replace all this text with your own text. You can remove any link to our website from this website template, you're free to use this website template without linking back to us. If you're having problems editing this website template, then don't hesitate to ask for help on the Forums."
        />
        <SmallCard
          title="OCEAN TRANSPORT"
          text="This website template has been designed by Free Website Templates for you, for free. You can replace all this text with your own text. You can remove any link to our website from this website template, you're free to use this website template without linking back to us. If you're having problems editing this website template, then don't hesitate to ask for help on the Forums."
        />
        <SmallCard
          title="AIR TRANSPORT"
          text="This website template has been designed by Free Website Templates for you, for free. You can replace all this text with your own text. You can remove any link to our website from this website template, you're free to use this website template without linking back to us. If you're having problems editing this website template, then don't hesitate to ask for help on the Forums."
        />
      </div>
    </div>
    <Footer />
  </div>
</template>
<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import LongCard from "../components/LongCard.vue";
import SmallCard from "../components/SmallCard.vue";

export default {
  name: "About",
  components: {
    Header,
    Footer,
    LongCard,
    SmallCard,
  },
};
</script>
<style>
.bodyAbout {
  height: 100%;
  width: 100%;
  background-color: #bbbbbb;
  display: flex;
  justify-content: center;
  min-height: 100vh;
  flex-direction: row;
  padding-bottom: 20px;
}
.group {
  display: flex;
  flex-direction: column;
  width: 25%;
  align-self: center;
}
@media only screen and (max-width: 600px) {
  .body{
    flex-direction: column;
  }
  .group{
    width: 90%;
  }
}
</style>
