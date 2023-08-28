<template>
  <div class="block-wrapper">
    <div class="block-left">
      <q-img class="circle" src="./../assets/profile-picture.png" />
    </div>
    <div class="block-right">
      <h1>Patrik Harmaňoš</h1>
      <h2>Web developer</h2>
      <div class="icon-block">
        <a class="icon"><q-icon name="ion-logo-github" size="36px"></q-icon></a>
        <a class="icon"
          ><q-icon name="ion-logo-linkedin" size="36px"></q-icon
        ></a>
        <a class="icon"
          ><q-icon name="ion-logo-instagram" size="36px"></q-icon
        ></a>
        <a class="icon"
          ><q-icon name="ion-logo-facebook" size="36px"></q-icon
        ></a>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.block-wrapper {
  display: flex;
  gap: 20px;

  .block-left {
    width: 40%;
    display: flex;
    align-items: center;
    justify-content: center;

    .circle {
      width: 200px;
      height: 200px;
    }
  }

  .block-right {
    width: 60%;
    color: #a3abb2;

    h1 {
      font-size: 42px;
      color: #f1f2f4;
      margin: 0;
      line-height: 42px;
    }

    h2 {
      font-size: 22px;
      margin: 10px 0;
    }

    .icon-block {
      display: flex;
      gap: 26px;

      .icon {
        color: #a3abb2;
        transition: color 0.3s ease-in-out;
        cursor: pointer;

        &:hover {
          color: #f1f2f4;
        }
      }
    }
  }
}
</style>
