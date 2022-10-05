<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Greet from "./components/Greet.vue";
import FullCalendar from "@fullcalendar/vue3";
import '@fullcalendar/core/vdom';
</script>

<template>
  <FullCalendar></FullCalendar>
</template>

<style scoped>
  FullCalendar{
    height: 500px;
    width: 100%;
  }
</style>
