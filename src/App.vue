<template>
  <HeaderComponent />
  <MainComponent />
  <SectionBlue />
  <FooterComponent />
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import SectionBlue from './components/SectionBlueComponent.vue';

export default {
  components: { HeaderComponent, MainComponent, FooterComponent, SectionBlue }
}
</script>

<style lang="scss" scoped>

</style>
