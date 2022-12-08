<template>
  <!-- <div>
    <Datepicker
      v-model="date"
      :format="'yyyy-MM-dd'"
      locale="id"
      :day-names="['Sen', 'Sel', 'Rab', 'Kam', 'Jum', 'Sab', 'Min']"
      auto-apply
      :hide-navigation="['calendar', 'time']"
      menu-class-name="custom-datepicker-style"
      range
    />
  </div> -->
  <Datepicker
    v-model="date"
    :format="'yyyy-MM-dd'"
    locale="id"
    :day-names="['Sen', 'Sel', 'Rab', 'Kam', 'Jum', 'Sab', 'Min']"
    auto-apply
    :hide-navigation="['calendar', 'time']"
    menu-class-name="custom-datepicker-style"
    inline
    range
  />
  <!-- <Datepicker
    style="margin-top: 20px"
    v-model="date"
    month-picker
    auto-apply
    :hide-navigation="['time']"
    inline
  /> -->
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
.dp__inner_nav {
  background-color: #3e7dc0;
  color: #fff;
  border-radius: 2.85px;
  margin-left: 8px;
  margin-right: 8px;
}
.dp__calendar_header_separator {
  display: none;
}
/* .dp__calendar */
</style>
