<template>
  <FullCalendar :options="calendarOptions" />
</template>

<script>
import FullCalendar from '@fullcalendar/vue'
import dayGridPlugin from '@fullcalendar/daygrid'
import interactionPlugin from '@fullcalendar/interaction'

export default {
  components: {
    FullCalendar, // make the <FullCalendar> tag available
  },
  data() {
    return {
      calendarOptions: {
        plugins: [dayGridPlugin, interactionPlugin],
        initialView: 'dayGridMonth',
      },
    }
  },
}
</script>
<style>
@import '../node_modules/@fullcalendar/common/main.css';
@import '../node_modules/@fullcalendar/daygrid/main.css';
@import '../node_modules/@fullcalendar/timegrid/main.css';
</style>
