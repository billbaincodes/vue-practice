<template>
  <view class="container">
    <text class="header">flô</text>
    <text class="text-color-primary">Email:</text>
    <text-input
      class="text-color-primary"
      :style="{height: 40, width: 300, borderColor: 'gray', borderWidth: 1}"
      v-model="myInput"
    />
    <text class="text-color-primary">Password:</text>
    <text-input
      class="text-color-primary"
      :style="{height: 40, width: 300, borderColor: 'gray', borderWidth: 1}"
      v-model="myInput"
    />
    <button
      class="text-color-primary"
      :on-press="logIn"
      title="myButton"
      color="#841584"
      accessibility-label="Learn more about this purple button"
    />
  </view>
</template>


<script>
export default {
  props: {
    navigation: {
      type: Object
    }
  },
  data() {
    return {
      myInput: ""
    };
  },
  methods: {
    logIn() {
      // this.myInput = "Button clicked!";
      this.navigation.navigate("Another");
    }
  }
};
</script>

<style>
.container {
  background-color: black;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.header {
  font-size: 80;
  letter-spacing: 10;
  color: cyan;
}
.text-color-primary {
  font-size: 20;
  color: white;
}
</style>
