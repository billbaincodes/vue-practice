
<template>
  <app-navigation></app-navigation>
</template>

<script>
import Vue from "vue-native-core";
import { VueNativeBase } from "native-base";

// registering all native-base components to the global scope of the Vue
Vue.use(VueNativeBase);



import { StackNavigator } from "vue-native-router";
import SplashScreen from './Splash.vue'
import MainScreen from './Main.vue'
import AnotherScreen from './Another.vue'

const AppNavigation = StackNavigator(
  {
    Main: MainScreen,
    Splash: SplashScreen,
    Another: AnotherScreen
  },
  {
    initialRouteName: 'Splash'
  }
);

export default {
    components: { AppNavigation }
}
</script>

<style>
.nav {
  font-size: 20;
  color: pink;
  background-color: black;
}
</style>