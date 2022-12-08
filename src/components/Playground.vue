<template>
  <div>
    <Datepicker
      v-model="date"
      :format="'dd-MM-yyyy'"
      locale="id"
      :day-names="['Sen', 'Sel', 'Rab', 'Kam', 'Jum', 'Sab', 'Min']"
      auto-apply
      :hide-navigation="['time']"
      menu-class-name="custom-datepicker-style"
    />
    <Datepicker
      style="margin-top: 20px"
      v-model="date2"
      month-picker
      auto-apply
      :hide-navigation="['time']"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Datepicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css';

const date = ref();
const date2 = ref();
</script>

<style>
/* .custom-datepicker-style {
  width: 400px;
} */

/* .dp__calendar_header */
/* .dp__calendar */
</style>
