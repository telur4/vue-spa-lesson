<template>
  <div>
    <Header></Header>
    <Nav></Nav>
    <HomeMain></HomeMain>
    <Footer></Footer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Header from '@/components/Header.vue';
import Nav from '@/components/Nav.vue';
import HomeMain from '@/components/HomeMain.vue';
import Footer from '@/components/Footer.vue';

@Component({
  components: {
    Header,
    Nav,
    HomeMain,
    Footer
  },
})
export default class Home extends Vue {}
</script>
