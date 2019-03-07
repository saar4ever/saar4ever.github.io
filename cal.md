---
layout: page
title: Calendar
subtitle: Jewish Young Adult Bay Area Events
---

<link href="//netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap-glyphicons.css" rel="stylesheet">
<!-- <link rel='stylesheet' href='https://bootswatch.com/3/paper/bootstrap.min.css' /> -->
<link rel='stylesheet' href='/css/bootstrap_paper.min.css' />
<link rel='stylesheet' href='/css/fullcalendar.css' />
<script src='/js/jquery.min.js'></script>
<script src='/js/moment.js'></script>
<script src='/js/fullcalendar.js'></script>
<script type='text/javascript' src='/js/gcal.js'></script>


<script>
  $(function() {
    $('#calendar').fullCalendar({
      header: {
        left: 'prev,next',
        center: 'title',
        right: 'month,listWeek'
      },
      themeSystem: 'bootstrap3',
      displayEventTime: true,
      eventLimit: true,
      height: 800,
      defaultView: 'month',
      fixedWeekCount: false,
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

<center><h5>Thank you <a href="https://www.facebook.com/Avirlila">Ella Gotesman</a> for helping keep the calendar up to date</h5></center>
