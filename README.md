Lack of @font-face Support Detection
=============

You can use this filter to selectively serve something else to browsers which don't support font embedding through @font-face.

Support
-------

#### Browsers Filtered

- Safari
- Chrome*
- Opera
- Gecko-based browsers

#### TODO

- Konqueror <sup><small>(coming soon)</small></sup>
- SVG format <small><sup>(planned)</sup></small>

Notes
-----

Internet Explorer supports @font-face since version 4.  
*Still* if you wanna target a specific version of IE you could use [downlevel-revealed conditional comments](http://en.wikipedia.org/wiki/Conditional_comment#Downlevel-revealed_conditional_comment) and add `||(!+"\v1")` to the filter.

<small>*except 4.0.249.2 &#9644;&#9654; 4.0.249.11</small>