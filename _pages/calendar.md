---
layout: page
title: Calendar
permalink: /calendar/
---

<link href="/assets/fullcalendar-4.3.1/packages/core/main.css" rel="stylesheet" />
<link href='/assets/fullcalendar-4.3.1/packages/daygrid/main.css' rel='stylesheet' />
<link href='/assets/fullcalendar-4.3.1/packages/list/main.css' rel='stylesheet' />

<script src="/assets/fullcalendar-4.3.1/packages/core/main.js"></script>
<script src='/assets/fullcalendar-4.3.1/packages/daygrid/main.js'></script>
<script src="/assets/fullcalendar-4.3.1/packages/google-calendar/main.js"></script>
<script src='/assets/fullcalendar-4.3.1/packages/list/main.js'></script>

<script>

      document.addEventListener('DOMContentLoaded', function() {
        var calendarEl = document.getElementById('calendar');

        var calendar = new FullCalendar.Calendar(calendarEl, {
            header: {
                left: 'today, prev,next',
                center: 'title',
                right: 'dayGridMonth,listMonth',
            },
            plugins: [ 'dayGrid', 'list', 'googleCalendar' ],
            googleCalendarApiKey: '{{ site.gcalendar_api_key }}',
            events: {
                googleCalendarId: 'robotics@utmsu.ca'
            },
            fixedWeekCount: false
        });

        calendar.render();
      });

</script>

<style>
    .fc-unthemed td.fc-today {
        background-color: rgb(230, 249, 255);
    }
</style>

<div id="calendar"></div>

[Add to Google Calendar](https://calendar.google.com/calendar?cid=robotics@utmsu.ca)