<script>
import FullCalendar from "@fullcalendar/vue3";
import dayGridPlugin from "@fullcalendar/daygrid";
import googleCalendarPlugin from "@fullcalendar/google-calendar";

export default {
  components: {
    FullCalendar, // make the <FullCalendar> tag available
  },
  data: function () {
    return {
      calendarOptions: {
        plugins: [dayGridPlugin, googleCalendarPlugin],
        initialView: "dayGridMonth",
        weekends: false,
        googleCalendarApiKey: "AIzaSyBvPvNygFXTYmp2E9uG_MwMIn5ZCGHSiw4",
        events: {
          googleCalendarId:
            "1108a61ce0013a3354a9ee8694003b7ba7a293c543c0b05a01916e6005f9acc9@group.calendar.google.com",
        },
      },
    };
  },
};
</script>

<template>
  <br />
  <h1>師傅派工</h1>
  <FullCalendar :options="calendarOptions" />
</template>

