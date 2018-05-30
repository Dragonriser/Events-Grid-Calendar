# Events-Grid-Calendar
These files are used to implement a basic grid calendar for the MS Cure Fund website's ["events"/"find programs" page](http://www.mscurefund.org/events). As of May 2018, NationBuilder does not have a default grid calendar view for events; this calendar setup aims to resolve this.
<img src="https://github.com/vickyjjj/Events-Grid-Calendar/blob/master/screenshots/june_test_popover.png?raw=true">

## Folders 
* **test**: test files for HTML/CSS/JS setup of basic grid calendar
* **site_files**: files uploaded to mscurefund.org website
* **screenshots**: screenshots of grid calendar view

## Instructions
To include SCSS styling for the calendar, include the following line in the **theme.scss** file:
```
@import "gridcal"
```

To set up the calendar view, before the for loop iterating over available events in the **events template** file, include the following line:
```
{% include "create_calendar_view" %}
```
Then, in the for loop of events, include the following line to add event blocks to the grid calendar view:
```
{% include "populate_calendar_view" %}
```

## Acknowledgments
* **Team Members**: Cleverina Cong, Daniela Guillen, Victoria Juan, Alex Tran (MIT '21)
* **Organizations**: [MIT Code for Good](http://codeforgood.mit.edu/), [MS Cure Fund](http://www.mscurefund.org/), [NationBuilder](https://nationbuilder.com/) 
* **Sources used**: [calendar with CSS grid](https://snook.ca/archives/html_and_css/calendar-css-grid)

