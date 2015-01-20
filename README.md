iCal2FullCalendar
=================

iCal2FullCalendar uses FullCalendar to render events created through
the iCalendar software. Simply export the calendar data as .ics/.ical
file and use the ics-convert.py python script to convert the .ics file
into a .json file. The conversion does NOT work for repeating event.

Dependencies:
=============

`pytz`, and `icalendar`

Python 2.6, 2.7 and 3.3+

Usage:
======
The script uses the follow iCalendar labels to format the .json file:

```html
(Required) TITLE:       Stores the title of the event.
(Optional) NOTES:       Stores the description of the event.
(Optional) URL:         Stores an URL to the event.
(Optional) LOCATION:    Stores the background color for the event
   FORMAT: [ #abc, #abcdef, rgb(64, 128, 255), or blue]
```

1. Create the calendar and save it as an .ical/.ics filel
2. Run "python ics-convert.py input output" on the .ical/.ics file.

Changelog:
==========

```html
1.0.0 - Public Release 
```