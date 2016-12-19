# visual-events
An interim js file that abstracts http protocols

Use this as a bookmarklet to load on any page to get a visual representation of javascript listeners attached to elements.

```
javascript:!function()%7bif(%22undefined%22!%3dtypeof%20VisualEvent)document.getElementById(%22Event_display%22)%3fVisualEvent.fnClose()%3aVisualEvent.fnInit()%3belse%7bvar%20e%3ddocument.createElement(%22script%22)%3be.setAttribute(%22language%22%2c%22JavaScript%22)%2ce.setAttribute(%22src%22%2cwindow.location.protocol%2b%27%2f%2frawgit.com%2fiam-decoder%2fvisual-events%2fmaster%2fsrc.js%27)%2cdocument.body.appendChild(e)%7d%7d()%3b
```


here is the un-minified/un-uriencoded bookmarklet:

```javascript: ! function() {
    if ("undefined" != typeof VisualEvent)
        document.getElementById("Event_display")
            ? VisualEvent.fnClose()
            : VisualEvent.fnInit();
    else {
        var e = document.createElement("script");
        e.setAttribute("language", "JavaScript"),
        e.setAttribute("src", window.location.protocol + '//rawgit.com/iam-decoder/visual-events/master/src.js'),
        document.body.appendChild(e)
    }
}();```
