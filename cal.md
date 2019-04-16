---
layout: page
title: Calendar
subtitle: Jewish Young Adult Bay Area Events
---

<!-- <link href="//netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap-glyphicons.css" rel="stylesheet"> -->
<!-- <link rel='stylesheet' href='https://bootswatch.com/3/paper/bootstrap.min.css' /> -->
<link rel='stylesheet' href='/css/bootstrap_paper.min.css' />
<link rel='stylesheet' href='/css/fullcalendar.css' />
<link rel='stylesheet' href='/css/main.css' />
<script src='/js/jquery.min.js'></script>
<script src='/js/moment.js'></script>
<script src='/js/fullcalendar.js'></script>
<script type='text/javascript' src='/js/gcal.js'></script>

<link rel='stylesheet' href='/css/jquery.qtip.min.css' />
<script type='text/javascript' src='/js/jquery.qtip.min.js'></script>

<script>
  $(function() {
    var tooltip = $('<div/>').qtip({
      id: 'fullcalendar',
      prerender: true,
      content: {
        text: ' ',
        title: {
          button: true
        }
      },
      position: {
        my: 'bottom center',
        at: 'top center',
        target: 'mouse',
        viewport: $('#calendar'),
        adjust: {
          mouse: false,
          scroll: false
        }
      },
      show: false,
      hide: false,
      style: 'qtip-tipped'
    }).qtip('api');
    
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

      eventClick: function(event, jsEvent, view) {
        var content = '<h6>'+event.title+'</h6>' + '<p><b>Description:</b> '+event.description;
        tooltip.set({'content.text': content}).reposition(jsEvent).show(jsEvent);
        return false;
      },
    });
    if($( document ).width() < 700){
      $('#calendar').fullCalendar('changeView', 'listWeek');
      $('#calendar').fullCalendar('option', 'height', 500);
    }
  });
</script>

<div id='calendar'></div>
<div id="popup"></div>

<center><font size="5"><a href="https://saarx.com/camp/">Join Camp Nai Nai Nai West</a></font></center>
<center><font size="3">Thank you <a href="https://www.facebook.com/Avirlila">Ella Gotesman</a> for helping keep the calendar up to date</font></center>

<link type="text/css" rel="stylesheet" href="/css/formCss.css"/>
<link type="text/css" media="print" rel="stylesheet" href="/css/printForm.css" />
<link type="text/css" rel="stylesheet" href="/css/nova.css" />
<link type="text/css" rel="stylesheet" href="/css/jotformtheme.css"/>
<style type="text/css">
    .form-label-left{
        width:150px;
    }
    .form-line{
        padding-top:6px;
        padding-bottom:6px;
    }
    .form-label-right{
        width:150px;
    }
    .form-all{
        width:650px;
        color:#3e4e1a !important;
        font-family:'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
        font-size:14px;
    }
    .form-radio-item label, .form-checkbox-item label, .form-grading-label, .form-header{
        color: false;
    }
</style>

<style type="text/css" id="form-designer-style">
    /* Injected CSS Code */
.form-label.form-label-auto {

        display: inline-block;
      float: left;
      text-align: left;

  }/*PREFERENCES STYLE*/
.form-all {
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}
.form-all .qq-upload-button,
.form-all .form-submit-button,
.form-all .form-submit-reset,
.form-all .form-submit-print {
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}
.form-all .form-pagebreak-back-container,
.form-all .form-pagebreak-next-container {
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}
.form-header-group {
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}
.form-label {
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}

.form-line {
  margin-top: 6px;
  margin-bottom: 6px;
}

.form-all {
  width: 650px;
}

.form-label-left,
.form-label-right,
.form-label-left.form-label-auto,
.form-label-right.form-label-auto {
  width: 140px;
}

.form-all {
  font-size: 14px
}
.form-all .qq-upload-button,
.form-all .qq-upload-button,
.form-all .form-submit-button,
.form-all .form-submit-reset,
.form-all .form-submit-print {
  font-size: 14px
}
.form-all .form-pagebreak-back-container,
.form-all .form-pagebreak-next-container {
  font-size: 14px
}

.supernova .form-all, .form-all {
  background-color: rgba(213,238,243,0.5);
  border: 1px solid transparent;
}

.form-all {
  color: #3e4e1a;
}
.form-header-group .form-header {
  color: #3e4e1a;
}
.form-header-group .form-subHeader {
  color: #3e4e1a;
}
.form-label-top,
.form-label-left,
.form-label-right,
.form-html,
.form-checkbox-item label,
.form-radio-item label {
  color: #3e4e1a;
}
.form-sub-label {
  color: #586834;
}

.supernova {
  background-color: rgba(255,255,255,0);
}
.supernova body {
  background: transparent;
}

.form-textbox,
.form-textarea,
.form-radio-other-input,
.form-checkbox-other-input,
.form-captcha input,
.form-spinner input {
  background-color: rgba(255,255,255,0.5);
}

.supernova {
  background-image: none;
}
#stage {
  background-image: none;
}

.form-all {
  background-image: none;
}

.ie-8 .form-all:before { display: none; }
.ie-8 {
  margin-top: auto;
  margin-top: initial;
}

  /*PREFERENCES STYLE*//*__INSPECT_SEPERATOR__*/
    /* Injected CSS Code */
</style>

<link type="text/css" rel="stylesheet" href="https://cdn.jotfor.ms/css/styles/buttons/form-submit-button-simple_green_apple.css?3.3.10333"/>
<form class="jotform-form nopad" action="https://submit.jotform.us/submit/90655184472159/" method="post" name="form_90655184472159" id="90655184472159" accept-charset="utf-8">
  <input type="hidden" name="formID" value="90655184472159" />
  <div class="form-all">
    <ul class="form-section page-section">
      <li id="cid_17" class="form-input-wide" data-type="control_head">
        <div class="form-header-group ">
          <div class="header-text httac htvam">
            <h2 id="header_17" class="form-header" data-component="header">
              <b>Missing Event?</b>
            </h2>
            <div id="subHeader_17" class="form-subHeader">
              Enter the event below and I will have it added to the calendar shortly <br/>
              Please enter your REAL NAME so I can contact you if I have questions on the event
            </div>
          </div>
        </div>
      </li>
      <li class="form-line jf-required" data-type="control_fullname" id="id_3">
        <label class="form-label form-label-left form-label-auto" id="label_3" for="first_3">
          Full Name
          <span class="form-required">
            *
          </span>
        </label>
        <div id="cid_3" class="form-input jf-required">
          <div data-wrapper-react="true">
            <span class="form-sub-label-container" style="vertical-align:top">
              <input type="text" id="first_3" name="q3_fullName[first]" class="form-textbox validate[required]" size="10" value="" data-component="first" required="" />
              <label class="form-sub-label" for="first_3" id="sublabel_first" style="min-height:13px"> First Name </label>
            </span>
            <span class="form-sub-label-container" style="vertical-align:top">
              <input type="text" id="last_3" name="q3_fullName[last]" class="form-textbox validate[required]" size="15" value="" data-component="last" required="" />
              <label class="form-sub-label" for="last_3" id="sublabel_last" style="min-height:13px"> Last Name </label>
            </span>
          </div>
        </div>
      </li>
      <li class="form-line jf-required" data-type="control_textbox" id="id_18">
        <label class="form-label form-label-left form-label-auto" id="label_18" for="input_18">
          Event Name
          <span class="form-required">
            *
          </span>
        </label>
        <div id="cid_18" class="form-input jf-required">
          <input type="text" id="input_18" name="q18_eventName" data-type="input-textbox" class="form-textbox validate[required]" size="20" value="" data-component="textbox" required="" />
        </div>
      </li>
      <li class="form-line jf-required" data-type="control_textbox" id="id_19">
        <label class="form-label form-label-left form-label-auto" id="label_19" for="input_19">
          Event Link
          <span class="form-required">
            *
          </span>
        </label>
        <div id="cid_19" class="form-input jf-required">
          <input type="text" id="input_19" name="q19_eventLink" data-type="input-textbox" class="form-textbox validate[required]" size="20" value="" data-component="textbox" required="" />
        </div>
      </li>
      <li class="form-line" data-type="control_textarea" id="id_16">
        <label class="form-label form-label-left form-label-auto" id="label_16" for="input_16"> Comments </label>
        <div id="cid_16" class="form-input">
          <span class="form-sub-label-container" style="vertical-align:top">
            <textarea id="input_16" class="form-textarea" name="q16_comments" cols="40" rows="3" data-component="textarea"></textarea>
            <label class="form-sub-label" for="input_16" style="min-height:13px"> Anything else I should know about this event? </label>
          </span>
        </div>
      </li>
      <li class="form-line" data-type="control_button" id="id_2">
        <div id="cid_2" class="form-input-wide">
          <div style="text-align:center" class="form-buttons-wrapper">
            <button id="input_2" type="submit" class="form-submit-button form-submit-button-simple_green_apple" data-component="button">
              Submit Form
            </button>
          </div>
        </div>
      </li>
      <li style="display:none">
        Should be Empty:
        <input type="text" name="website" value="" />
      </li>
    </ul>
  </div>
</form>
<!-- <script src='/js/jquery-3.3.1.min.js' type="text/javascript"></script> -->
<script src='/js/jquery.maskedinput.min.js' type="text/javascript"></script>
<script src='/js/maskedinput.min.js' type="text/javascript"></script>
<!-- <script src='/js/prototype.forms.js' type="text/javascript"></script> -->
<script src='/js/jotform.forms.js' type="text/javascript"></script>
<script type="text/javascript">
   JotForm.setConditions([{"action":[{"field":"21","visibility":"Show","id":"action_0_1551310672039"}],"id":"1551310644216","index":"0","link":"Any","priority":"0","terms":[{"field":"11","operator":"equals","value":"Other"}],"type":"field"}]);
	JotForm.init(function(){
      JotForm.setPhoneMaskingValidator( 'input_22_full', '(###) ###-####' );
      setTimeout(function() {
          $('input_9').hint('ex: myname@example.com');
       }, 20);
    /*INIT-END*/
	});
</script>
<script type="text/javascript">JotForm.ownerView=true;</script>