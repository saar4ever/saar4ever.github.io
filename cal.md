---
layout: page
title: Calendar
subtitle: Jewish Young Adult Bay Area Events
---

<link rel='stylesheet' href='/css/fullcalendar.css' />
<script src='/js/jquery.min.js'></script>
<script src='/js/moment.js'></script>
<script src='/js/fullcalendar.js'></script>
<script type='text/javascript' src='/js/gcal.js'></script>
<link href='https://bootswatch.com/3/paper/bootstrap.min.css' rel='stylesheet' />


<script>
  $(function() {
    $('#calendar').fullCalendar({
      header: {
        left: 'prev,next today',
        center: 'title',
        right: 'month,listWeek'
      },
      themeSystem: 'bootstrap3',
      displayEventTime: true,
      eventLimit: true,
      height: 800,
      defaultView: 'month',
      googleCalendarApiKey: 'AIzaSyAFJI5E7tJ3y143JM3ZWrzTWlScQxNQntg',
      events: 'bsp4pl7nrmbt1merbkuehqluj4@group.calendar.google.com',
      eventClick: function(event) {
        window.open(event.url, '_blank', 'width=700,height=600');
        return false;
      }
    });
    if($( document ).width() < 700){
       $('#calendar').fullCalendar('changeView', 'listWeek');
    }
  });
</script>

<div id='calendar'></div>

# The Calendar 4.0
