<template>
  <div class="block-wrapper">
    <q-btn-group class="button-group">
      <q-btn
        class="button"
        :style="{
          'background-color': !btn1.active ? '#171f26' : '#0C151D',
          color: '#A3ABB2',
        }"
        :label="btn1.label"
        @click="
          btn1.active = true;
          btn2.active = false;
        "
      ></q-btn>
      <q-btn
        class="button"
        :style="{
          'background-color': !btn2.active ? '#171f26' : '#0C151D',
          color: '#A3ABB2',
        }"
        :label="btn2.label"
        @click="
          btn1.active = false;
          btn2.active = true;
        "
      ></q-btn>
    </q-btn-group>
  </div>

  <div v-if="btn1.active">skola</div>

  <div v-if="btn2.active">praca</div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
const btn1 = ref({
  label: 'Vzdelanie',
  color: 'secondary',
  active: true,
});

const btn2 = ref({
  label: 'Pracovné skúsenosti',
  color: 'secondary',
  active: false,
});
</script>

<style lang="scss" scoped>
.block-wrapper {
  background-color: #171f26;
  border-radius: 20px;
  margin-top: 40px;

  .button-group {
    padding: 15px;
    width: 100%;
    display: flex;
    gap: 15px;
    background-color: #171f26;
    border-radius: 20px;

    .button {
      width: 50%;
      padding: 15px 0;
      background-color: #171f26;
      border-radius: 10px;
      font-size: 16px;
    }
  }
}
</style>
