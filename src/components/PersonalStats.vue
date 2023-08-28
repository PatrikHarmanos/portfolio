<template>
  <div class="block-wrapper">
    <div class="block">
      <b>Ahojte.</b> ipsum dolor sit, amet consectetur adipisicing elit. Fugiat
      impedit quia ea ullam et dolorem! Fugiat inventore ducimus, culpa sequi
      fugit in ipsa praesentium debitis! Vitae officia eaque quia molestias!
    </div>

    <div class="block-buttons">
      <q-btn
        class="button button-left"
        icon-right="download"
        label="Download CV"
      />
      <q-btn class="button button-right" label="Contact me" />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.block-wrapper {
  gap: 90px;
  padding: 20px;
  color: #a3abb2;
  font-size: 22px;
  margin-top: 50px;

  .block {
    text-align: justify;
    margin-bottom: 50px;
  }

  .block-buttons {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    gap: 40px;
    margin: 0 10px;

    .button {
      text-transform: capitalize;
      font-size: 18px;
      width: 50%;
      padding: 20px;
      border-radius: 10px;
    }

    .button-left {
      background-color: #ffe071;
      color: #3d3d3d;
    }

    .button-right {
      background-color: #171f26;
      color: #a3abb2;
    }
  }
}
</style>
