Lack of @font-face Support Detection
=============

You can use this filter to selectively serve something else to browsers which don't support TTF/OTF/WOFF embedding through @font-face.

Support
-------

#### Browsers Filtered

- Safari
- Chrome¹
- Opera
- Gecko-based browsers
- Konqueror²

#### TODO

- SVG format <small><sup>[planned]</sup></small>

Notes
-----

Internet Explorer supports @font-face since version 4.  
Still if you wanna target a specific version of IE you could use [downlevel-revealed conditional comments](http://en.wikipedia.org/wiki/Conditional_comment#Downlevel-revealed_conditional_comment) and add `||(!+"\v1")` to the filter.

Reminder: ids can potentially [pollute the global scope](https://www.w3.org/Bugs/Public/show_bug.cgi?id=11960) so remember to avoid naming them chrome, opera or konqueror.

<small>¹ except 4.0.249.2–11  
² except 4.3 ß1–RC1</small>