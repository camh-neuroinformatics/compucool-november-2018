# scwg

Tools and Frameworks:
- Jekyll
- MaterializeCSS
- FullCalendarJS

Layouts:
- put layout name in YAML front matter in order to use that layout
- two layouts
- default layout (used for most pages)
- course description (used for course description collapsibles)

Includes:
- includes used throughout to make code cleaner
- sometimes variables passed in to them

Collections:
- collections used to describe courses
- one collection per day courses are taught
- each folder for a collection must contain course files, named in the following pattern (0-indexed): 00-name-of-course.html
- numbering is important, and should follow chronological order
- add new collections (days courses are taught on) into _config.yml

Calendar feed:
- json file, just follow the example
- id number is important: 0-indexed course IDs should be chronologically ordered, and match the order you want the courses to appear on the index page
- if id number is not correct or out of order, clicking on an event in the calendar will not open the correct collapsible
