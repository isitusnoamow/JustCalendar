<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Greet from "./components/Greet.vue";
import FullCalendar from "@fullcalendar/vue3";
import '@fullcalendar/core/vdom';
import dayGridPlugin from '@fullcalendar/daygrid'
import interactionPlugin from '@fullcalendar/interaction'

</script>

<script>
export default {
  components: {
    FullCalendar
  },
  data() {
    return {
      calendarOptions: {
        plugins: [ dayGridPlugin, interactionPlugin ],
        initialView: 'dayGridMonth'
      }
    }
  }
}
</script>

<template>
  <div id="view">
    <FullCalendar :options="calendarOptions" />
  </div>
</template>

<style scoped>
  #view{
    max-width: 100%;
    max-height: 100%;
  }
</style>
