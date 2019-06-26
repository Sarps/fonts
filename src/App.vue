<template>
  <v-app>
    <TopNav class="white"/>
    <v-content app class="white">
      <v-container fluid grid-list-xl>
        <v-layout row wrap>
          <FontCard v-for="i in 5" :key="i"/>
        </v-layout>
      </v-container>
    </v-content>
    <SideNav/>
  </v-app>
</template>

<script>

import FontCard from './components/FontCard'
import TopNav from './components/TopNav'
import SideNav from "./components/SideNav";

export default {
  name: 'App',
  components: {
    FontCard, TopNav, SideNav
  },
  data () {
    return {
      //
    }
  }
}
</script>
