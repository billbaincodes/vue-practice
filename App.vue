
<template>
  <app-navigation class="nav"></app-navigation>
</template>

<script>
import { StackNavigator } from "vue-native-router";
import SplashScreen from './Splash.vue'
import MainScreen from './Main.vue'

const AppNavigation = StackNavigator(
  {
    Splash: SplashScreen,
    Main: MainScreen
  },
  {
    initialRouteName: 'Splash',
  }
);

export default {
    components: { AppNavigation }
}

</script>

<style>
.nav{
  font-size: 20;
  color: pink;
  background-color: black;
}
</style>