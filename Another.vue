<template>
  <nb-container>
    <nb-header hasTabs/>
    <nb-tabs>
      <nb-tab heading="Profile">
        <tab-one />
      </nb-tab>
      <nb-tab heading="Run">
        <tab-two />
      </nb-tab>
      <nb-tab heading="Music">
        <tab-three />
      </nb-tab>
    </nb-tabs>
  </nb-container>
</template>
<script>
import TabOne from "./components/tabOne";
import TabTwo from "./components/tabTwo";
import TabThree from "./components/tabThree";
export default {
  components: { TabOne, TabTwo, TabThree }
};
</script>




<style>
.icon-star {
  font-size: 15;
  color: #fff;
  line-height: 20;
}
.badge-custom-bg {
  background-color: black;
}
</style>