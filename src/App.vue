<template>
  <HeaderComponent />
  <JumboComponent />
  <MainComponent />
  <SectionBlue />
  <FooterComponent />
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import JumboComponent from './components/JumboComponent.vue';
import MainComponent from './components/MainComponent.vue';
import SectionBlue from './components/SectionBlueComponent.vue';

export default {
  components: { HeaderComponent, MainComponent, FooterComponent, SectionBlue, JumboComponent }
}
</script>

<style lang="scss" scoped>

</style>
