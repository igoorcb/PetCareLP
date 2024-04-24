<template>
  <HeaderComponent/>
  <CentralModal/>
  <About/>
  <Growth/>
  <Clients/>
  <FooterPet/>
</template>

<script>
import HeaderComponent from './components/Header/HeaderComponent.vue';
import CentralModal from './components/CentralModal/CentralModal.vue';
import About from './components/About/About.vue';
import Growth from './components/Growth/Growth.vue';
import Clients from './components/Clients/Clients.vue';
import FooterPet from './components/FooterPet/FooterPet.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    CentralModal,
    About,
    Growth,
    Clients,
    FooterPet,
  },
};
</script>


