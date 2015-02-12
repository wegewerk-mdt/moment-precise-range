Moment Date Range Plugin
========================

This is a plugin for the momentjs Javascript Library.
It adds a function to display the difference between 2 dates precisely.

It is a fork from http://codebox.org.uk/pages/moment-date-range-plugin

I added locale Support and short notation support

Example
-------

<code language="javascript">
    a = moment("2013-02-08 09:30:26");
    b = moment("2013-02-08 12:35:00");

    # default behaviour
    moment.locale('en');
    moment.preciseDiff(a,b);
    #"3 hours 4 minutes a few seconds"

    # set other locale
    moment.locale('de');
    moment.preciseDiff(a,b);
    #"3 Stunden 4 Minuten ein paar Sekunden"

    # short format (no i18n support)
    moment.preciseDiff(a,b,{hour:true,minute:true,short:true})
    # "3h 4min"
</code>

Installation
------------

`bower install git@github.com:wegewerk-mdt/moment-precise-range.git --save`

```html
<script src="bower_components/moment/moment.js"></script>
<script src="bower_components/moment-precise-range/readable-range.js"></script>
```
