<template>
  <kinesis-container class="fixed-bg" :duration="1000">
    <kinesis-element
      :strength="10"
      :cycle="2"
      type="transform"
      style="position: relative"
    >
      <kinesis-element :strength="9" :cycle="1" type="depth">
        <img src="../assets/img/shadow2.svg" />
      </kinesis-element>
      <kinesis-element
        :strength="10"
        type="depth_inv"
        style="position: absolute; top: 0"
      >
        <img src="../assets/img/logo2.svg" />
      </kinesis-element>
    </kinesis-element>
  </kinesis-container>
</template>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>
<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}
.fixed-bg {
  position: absolute;
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 0;
  top: 0;
}
@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
