<script setup lang="ts">
import { ref } from 'vue'
import NavBar from './components/NavBar.vue'
import MainContent from './components/MainContent.vue'
const components = {
  'nav-bar': NavBar,
  'main-content': MainContent
}
</script>

<template>
  <nav-bar></nav-bar>
  <main-content></main-content>
</template>

<style lang="scss">
@import './styles/1-base/base-dir.scss';
@import './styles/2-layouts/layout-dir.scss';
@import './styles/3-modules/modules-dir.scss';
@import './styles/4-responsive/responsive-dir.scss';
</style>
