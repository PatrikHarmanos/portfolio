<template>
  <div class="block-wrapper">
    <div class="switcher" @click="changeText()">
      <span>{{ country }}</span>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
const country = ref('sk');

function changeText() {
  country.value = country.value === 'sk' ? 'en' : 'sk';
}
</script>

<style lang="scss" scoped>
.block-wrapper {
  width: 100%;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 120px;
  margin-top: 15px;
  margin-bottom: 50px;

  .switcher {
    background: #171f26;
    width: 80px;
    height: 80px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    font-size: 20px;
    font-weight: 500;
    color: #a3abb2;
    transition: 0.3s ease-in-out;

    .img {
      height: 25px;
    }

    &:hover {
      background: #1e2a33;
    }
  }
}
</style>
