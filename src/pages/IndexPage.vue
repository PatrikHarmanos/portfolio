<template>
  <q-page class="body row">
    <div class="body-inner">
      <language-switcher />

      <personal-header />

      <personal-stats />

      <tabs-component />
    </div>
  </q-page>
</template>

<script setup lang="ts">
import LanguageSwitcher from 'src/components/LanguageSwitcher.vue';
import PersonalHeader from 'src/components/PersonalHeader.vue';
import PersonalStats from 'src/components/PersonalStats.vue';
import TabsComponent from 'src/components/TabsComponent.vue';
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');

.body {
  background-color: #0c151d;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  font-family: 'Poppins', sans-serif;

  .body-inner {
    width: 600px;
  }
}
</style>
