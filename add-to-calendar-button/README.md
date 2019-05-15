This "Add to Calendar" button is an adaptation of the [OuiCal JS library](https://github.com/carlsednaoui/add-to-calendar-buttons) for NationBuilder websites. When implemented on event pages, an RSVP can click a button to add the event to their personal Google, iCal, Outlook, or Yahoo calendar.

## How to Implement
1. Download the `ouical.js`, `main.css`, and `_add_to_calendar_button.html` files from this Github repo. Upload those files to your NationBuilder wesbite's [custom theme](https://nationbuilder.com/theme_documentation).
2. Right before the closing `</head>` tag in `layout.html`, import the OuiCal files, like so:
```
<script src="ouical.js"></script>
<link rel="stylesheet" href="main.css">
```
3. Add the snippet `{% include "add_to_calendar_button" %}` to your `pages_show_event.html` and `pages_show_event_wide.html` theme templates. It's up to you where you'd like the button to go, but I'd recommend add the button after the WHEN and WHERE sections.
