
<template>
  <view>
    <tab-nav></tab-nav>
  </view>
</template>

<script>
import Vue from "vue-native-core";
import { VueNativeBase } from "native-base";

// registering all native-base components to the global scope of the Vue
Vue.use(VueNativeBase);

import { TabNavigator, TabBarBottom, StackNavigator } from "vue-native-router";
import SplashScreen from "./Splash.vue";
import MainScreen from "./Main.vue";
import AnotherScreen from "./Another.vue";
import HomeScreen from "./screens/HomeScreen.js";
import LinksScreen from "./screens/LinksScreen.js";
import SettingsScreen from "./screens/SettingsScreen.js";

const tabNav = TabNavigator(
  {
    Home: HomeScreen,
    Settings: SettingsScreen
  },
  {
    tabBarPosition: "bottom",
    tabBarComponent: TabBarBottom
  }
);

export default {
  beforeCreate() {
    console.log("butts");
  },
  components: {
    tabNav
  }
};
</script>

<style>
.nav {
  font-size: 20;
  color: pink;
  background-color: black;
}
</style>