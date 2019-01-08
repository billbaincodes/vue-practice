<template>
  <nb-container>
    <nb-header/>
    <nb-content padder>
      <nb-badge>
          <nb-text>2</nb-text>
      </nb-badge>
      <nb-badge primary>
          <nb-text>2</nb-text>
      </nb-badge>
      <nb-badge success>
          <nb-text>2</nb-text>
      </nb-badge>
      <nb-badge info>
          <nb-text>5</nb-text>
      </nb-badge>
      <nb-badge warning>
          <nb-text>2</nb-text>
      </nb-badge>
      <nb-badge danger>
          <nb-text>2</nb-text>
      </nb-badge>
      <nb-badge primary>
          <nb-icon name="star" class="icon-star" />
      </nb-badge>
      <nb-badge class="badge-custom-bg">
          <nb-text>1866</nb-text>
      </nb-badge>
    </nb-content>
  </nb-container>
</template>




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