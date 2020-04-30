# uuBookKit-ext
## Features
Additional links and icons in the page:
- Page title is a link to Knowledge Base
- Pencil icon for editing a document structure is added (if user has permissions)
- MD link for editing document in [uuDockitHelper](https://github.com/jiridudekusy/uuDockitHelper) is added (if used has permissions)
- Pencil icon for editing each section is added (if user has the permission)
- Clickable table of content is shown at the top of each page. It can be enabled/disabled using the ToC icon near the book title.
- Refresh icon, which refreshes just current page content (not the whole web page).

Other features:
- Quick search field at the top of the page supporting fulltext search of the page titles
- Menu
  - Long names in menu do not wrap (full name is displayed by moving cursor over a menu item)
  - Width of left navigation menu can be resized using drag & drop.
  - Specific menu items are colored (Business, uuSubApp, *Stores, uuCMD)
- Scenarios
  - Add option to copy HDS and alternative scenarios with ordering numbers as a program comments into clipboard.

Keyboard shortcuts:
- *ESC* closes edit window.
- *E* starts edit mode of the page and all its sections.
- *Shift+E* does the same as *E* and additionally starts edit mode of all sub-sections. This make take a couple of seconds for a page with a complex structure! And it also does not work in all cases, because some sub-sections are loaded lazily.
- *Ctrl+S* saves the data in edit mode and ends the edit mode. 
- *Ctrl+Q* or *Alt+N* or *Alt+Shift+N* (depending on browser) focuses the quick search field at the top of the page.
- *F4* refreshes just current page content (not the whole web page).

## Installation
1. Add https://tampermonkey.net/ into your browser (supported for Chrome, Firefox, Edge, Safari, tested for Chrome, Firefox).
2. Install User script from this URL: [uubookkit-ext.user.js](https://github.com/pavel-zeman/uubookkit-ext/raw/master/uubookkit-ext.user.js)

## Configuration
- In case of [uuDockitHelper](https://github.com/jiridudekusy/uuDockitHelper) is executed on different IP or port than http://localhost:4323/vendor-app-subapp/0-0/editor (the default port could be 1234) please edit the `mdUrl` in script. 
