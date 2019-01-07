<template>
  <view class="container">
    <text class="text-color-primary">{{ myInput }}</text>
    <text class="text-color-primary">CandyCanes</text>

    <text-input
      class="text-color-primary"
      :style="{height: 40, width: 150, borderColor: 'gray', borderWidth: 1}"
      v-model="myInput"
    />
    <button
      class="text-color-primary"
      :on-press="handleButton"
      title="myButton"
      color="#841584"
      accessibility-label="Learn more about this purple button"
    />
    <!-- <text-input :style="{height: 40, borderColor: 'gray', borderWidth: 1}" v-model="text"/> -->
  </view>
</template>


<script>
export default {
  data() {
    return {
      message: "Hello there world",
      myInput: ""
    };
  },
  methods: {
    handleButton() {
      this.myInput = "Button clicked!";
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
.text-color-primary {
  font-size: 20;
  color: cyan;
}
</style>
