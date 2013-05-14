Flat-UI-Pro-Support
===================

Flat UI Pro Support
http://designmodo.com/flat/

Use this repo to submit your issues and bugs and we will be glad to solve your questions. We want to make our product better and very soon we will release some updates for you. Thank you for your help!


What is Flat UI?
================
[Flat UI](http://designmodo.com/flat) is a beautiful theme for [Bootstrap](http://getbootstrap.com/). We redesigned many of it's components to look flat in every pixel.

However, to make form and some other elements look exactly how we want we ended up using JS plugins which means it requires a little more efforts integrating them into your project.


How to Use It?
===============
Since it is built on top of Bootstrap as a theme you can use it on your project with Bootstrap (tested on [2.3.1](http://github.com/twitter/bootstrap/tree/v2.3.1)). We did not modify any line of Bootstrap so you will be safe using Flat UI in your ongoing project (unless you hacked it :)

We provide you with CSS and [Less](http://lesscss.org/) sources.

1. Using CSS is as easy as dropping `css/flat-ui.css` to your project folder and including it in your template/html page: `<link href="css/flat-ui.css" rel="stylesheet">`
2. Use Less if you want to modify/extend Flat UI in your project. We built it Bootstrap way so you won't find big difference.

The easiest way to start is by using our start-up `template.html` where all files are already included and ready to be used (JS plugins are included, but not initialized for no need).


File Structure
==============
Once purchased, unzip the compressed archive to see the structure:

    flat-ui/
    ├── bootstrap/
    ├── css/
    │   └── flat-ui.css
    ├── fonts/
    ├── images/
    ├── js/
    └── less/
      ├── config.less
      ├── flat-ui.less
      ├── icon-font.less
      ├── mixins.less
      ├── spaces.less
      └── modules/

Let's go from top to the bottom of this list.

**bootstrap/** — as you can guess this is a folder where all original Bootstrap files are (untouched). Before using our theme please make sure you didn't modify anything that can break compatibility: paddings, margins, etc. 
*Note*: you can modify `variables.less` safely.

**css/** — compiled Flat UI CSS. If you like everything and don't want to change the look of our components it is better to use CSS version. This is an easiest way to start using Flat UI.

**fonts/** — yes, this is an icon font. When integrating make sure you copied all font files correctly. You might want to change/add glyphs. If so, open [IcoMoon](http://icomoon.io/app) and import `icomoon-session.json` there to make all glyhps editable.

![IcoMoon](images/ico-moon.png?raw=true)

**images/** — unfortunately we should use them in few cases. The rest is in the glyphs.

**js/** — we tried hard to make our components all look true Flat. To do so we used JS plugins. Most of them are well known, some of them not. The most JS-ified part is form components: checkboxes, radios, switches, selects since it is not currently possible to style them identically in all browsers. Open `application.js` for integration examples.

**less/** — where all our stylesheets are (not preprocessed).
`config.less` is where all variables are.
`flat-ui.less` links everything into one single bundle.
`icon-font.less` makes all icon glyphs work. Converted by IcoMoon.
`mixins.less` helps automating things. Feel free to add yours here.
`modules/` is where all components are. If you want to add yours create module-name.less here. Name it as a class name if possible.


New Components
==============
`bottom.less` Bottom menus and footer.

`checkbox-and-radio.less` Custom checkboxes and radios.

`dialog.less` Used for system messages.

`iconbar.less` Icon bar (another navigation type).

`select.less` Custom selects.

`switch.less` Custom switch.

`tagsinput.less` Tags input field.

`ui-datepicker.less` Datepicker widget.

`ui-slider.less` Range slider.

`ui-spinner.less` Text input with increment/decrement.


Components restyled
===================
`alerts.less`

`breadcrumbs.less`

`buttons.less`

`caret.less`

`dropdown.less`

`input.less`

`label-badges.less`

`nav.less`

`navbar.less`

`pager.less`

`pagination.less`

`popover.less`

`progress.less`

`tables.less`

`tooltip.less`

`type.less`
