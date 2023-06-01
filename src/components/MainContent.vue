<script setup lang="ts">
import { ref } from 'vue'
import SearchBox from './SearchBox.vue'

import AsideComponent from './AsideComponent.vue'
import MainTools from './MainTools.vue'

const components = {
  'search-box': SearchBox,

  'aside-component': AsideComponent,
  'main-tools': MainTools
}
</script>

<template>
  <div id="main-content">
    <search-box></search-box>
    <div class="mainwithaside">
      <main class="main">
        <main-tools></main-tools>
      </main>
      <aside class="aside">
        <aside-component></aside-component>
      </aside>
    </div>
  </div>
</template>
