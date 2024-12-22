<script>
import Header from './components/Header.vue';
import Wrap from './components/Wrap.vue';
import AboutUs from './components/AboutUs.vue';
import DevTitle from './components/DevTitle.vue';
import Dev from './components/Dev.vue';
import Trust from './components/Trust.vue';
import TrustInfo from './components/TrustInfo.vue';
import Organize from './components/Organize.vue';
import Map from './components/Map.vue';
import Footer from './components/Footer.vue';


export default {
  components: {
    Header,
    Wrap,
    AboutUs,
    DevTitle,
    Dev,
    Trust,
    TrustInfo,
    Organize,
    Map,
    Footer,


  }
}

</script>

<template>
  <Header />
  <Wrap />
  <div class="aboutus">
    <AboutUs />
  </div>
  <DevTitle />
  <Dev />
  <Trust />
  <TrustInfo />
  <Organize />
  <Map />
  <Footer />

</template>

<style scoped>
.aboutus {
  margin-bottom: 12em;
}

</style>
