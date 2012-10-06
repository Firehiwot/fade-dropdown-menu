CSS3 Dropdown with Fade
========================

In the past, dropdown menus were only possible through Javascript. Nowadays we can use CSS3 to achieve pretty much every traditional dropdown effect.

This dropdown menu is [semantic][sem] & entirely CSS3.

[View it live.][sbc]

[sem]: http://en.wikipedia.org/wiki/Semantic_Web "Semantic Web"
[sbc]: http://jmeas.com/projects/git/dd1/menu.html  "CSS3 Dropdown with Fade"

### Compatibility

This is 100% compatible with Chrome, Safari, Opera, and Firefox. Note that a little nuance in the CSS is needed for the fade to work with Firefox. It's noted in the CSS file. I also included the [iOS :hover double-click feature][click].

[click]: http://www.nczonline.net/blog/2012/07/05/ios-has-a-hover-problem/ "iOS Double Click"

This will function on IE6+, but it won't display as nicely in IE as in those other browsers.

Firstly, none of the transitions work in Internet Explorer, even IE9 (remember, IE doesn't support transitions of any sort. This incompatibility isn't unique to this dropdown).

Secondly, the CSS3 arrows will only display in IE8+. This is for a few reasons. Firstly, we use a CSS unicode character that I don't think is supported pre-IE8. We also use the ::after pseudoelement to display the triangle; again, IE8+. And we're transforming the arrow, which, yet again, is only IE8+.

If you remove those pesky CSS arrows, it will otherwise display correctly in IE6+ (aside from the transitions).

### Technical details

I used a unicode character for the triangle instead of CSS borders. You might be wondering why this is. In Firefox, the border hack for CSS triangles displays black bars along the edges of the triangle when it isn't entirely opaque. These aren't there when it's viewed at 1 opacity, so you never notice in typical usage. But, since this has a fade...yeah. You get the picture.

Enjoy!
