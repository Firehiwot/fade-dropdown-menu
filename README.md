CSS3 Dropdown with Fade
========================

In the past, dropdown menus were only able to be made with Javascript. With CSS3, we can replace all of the JS with CSS and get the same effects.

This dropdown is semantic, entirely CSS, and has a fade effect.

[View it live.][sbc]

[sbc]: http://jmeas.com/projects/git/dd1/menu.html  "CSS3 Dropdown with Fade"

### Usage

A common usage would be having the dropdown appear over other elements on your site. The code I've given here doesn't include this, but it isn't hard to add. All you need to do is make sure that the submenu ULs have a higher z-index than the element you want it appear over. If you want it to be above everything else on your page, it'll be pretty safe to just assign a z-index value of, say, 1000 to those submenu ULs.

### IE Compatibility

In the form it's given in, this will only display properly on IE8+ (as long as you declare a doctype, which you should, anyway).

If you remove the CSS arrows, this will work on IE6+.
