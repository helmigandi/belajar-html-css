## Position and Layout
1. Static
HTML elements are positioned static by default.


2. Relative
We can shift the element around the page.
Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position.

3. Fixed
An element with `position: fixed;` is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

4. Absolute
An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

![absolute](https://github.com/helmiz/belajar-html-css/blob/master/part6%20CSS%20Layout%20%26%20Position/img/absolute.png "absolute")


5. Sticky
An element with position: sticky; is positioned based on the user's scroll position.
A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).

