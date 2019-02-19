---
layout: page
title: Calendar 
subtitle: Jewish Young Adult Bay Area Events
---

<link rel='stylesheet' href='fullcalendar/fullcalendar.css' />
<script src='lib/jquery.min.js'></script>
<script src='lib/moment.min.js'></script>
<script src='fullcalendar/fullcalendar.js'></script>
<script type='text/javascript' src='fullcalendar/gcal.js'></script>

<script>
  $(function() {
    $('#calendar').fullCalendar({
      header: {
        left: 'prev,next today',
        center: 'title',
        right: 'month,listYear'
      },
      displayEventTime: false, // don't show the time column in list view
      googleCalendarApiKey: 'AIzaSyDcnW6WejpTOCffshGDDb4neIrXVUA1EAE',
      // US Holidays
      events: 'en.usa#holiday@group.v.calendar.google.com',
      eventClick: function(event) {
        // opens events in a popup window
        window.open(event.url, '_blank', 'width=700,height=600');
        return false;
      }
    });
  });
</script>


</div><div id='calendar'></div>

# The Past v3.1

<div class="responsive-iframe-container small-container"><iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;showTabs=0&amp;showCalendars=0&amp;mode=AGENDA&amp;height=800&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=bsp4pl7nrmbt1merbkuehqluj4%40group.calendar.google.com&amp;color=%23182C57&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="700" height="600" frameborder="0" scrolling="no"></iframe></div>
<div class="responsive-iframe-container big-container"><iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;showTabs=0&amp;showCalendars=0&amp;height=800&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=bsp4pl7nrmbt1merbkuehqluj4%40group.calendar.google.com&amp;color=%23182C57&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="1000" height="700" frameborder="0" scrolling="no"></iframe></div>

### Calendar
