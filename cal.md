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

<script>
  $(function() {
    $('#calendar').fullCalendar({
      header: {
        left: 'prev,next',
        center: 'title',
        right: 'today'
      },
      displayEventTime: true,
      <!-- defaultView: 'listWeek', -->
      googleCalendarApiKey: 'AIzaSyAFJI5E7tJ3y143JM3ZWrzTWlScQxNQntg',
      events: 'bsp4pl7nrmbt1merbkuehqluj4@group.calendar.google.com',
      eventClick: function(event) {
        window.open(event.url, '_blank', 'width=700,height=600');
        return false;
      }
    });
  });
</script>

<div class="small-container">
    <script>
    <!-- document.write("why isnt it working"); -->
    var height = $( document ).width();
    document.write("Width is - " + height);
        $(function() {
            if($("div").height() == 300){
                document.write("not doing this");
                $('#calendar').fullCalendar('changeView', 'listWeek');
            }
        });
    </script>
    <!-- Goodbye Earth -->
</div>
<!-- var locale = $('#calendar').fullCalendar('option', 'locale'); -->


<div class="big-container">
    <!-- <script>
        $(function() {
            $('#calendar').fullCalendar('changeView', 'listWeek');
        });
    </script> -->
    Hello World
</div>

<div id='calendar'></div>


# The Past v3.6

<!-- <div class="responsive-iframe-container small-container"><iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;showTabs=0&amp;showCalendars=0&amp;mode=AGENDA&amp;height=800&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=bsp4pl7nrmbt1merbkuehqluj4%40group.calendar.google.com&amp;color=%23182C57&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="700" height="600" frameborder="0" scrolling="no"></iframe></div>
<div class="responsive-iframe-container big-container"><iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;showTabs=0&amp;showCalendars=0&amp;height=800&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=bsp4pl7nrmbt1merbkuehqluj4%40group.calendar.google.com&amp;color=%23182C57&amp;ctz=America%2FLos_Angeles" style="border-width:0" width="1000" height="700" frameborder="0" scrolling="no"></iframe></div> -->

### Calendar
