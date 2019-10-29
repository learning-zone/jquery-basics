## jQuery functions 


#### JQUERY SELECTORS


|Sl.No|Selector            |  Example               |     Selects                |
|---|----------------------|------------------------|----------------------------|
|01.|*                      |$("*")                     |All elements|
|02.|#id                    |$("#lastname")             |The element with id="lastname"|
|03.|.class                 |$(".intro")                |All elements with class="intro"|
|04.|.class,.class          |$(".intro,.demo")          |All elements with the class "intro" or "demo"|
|05.|element                |$("p")                     |All `<p>` elements|
|06.|el1,el2,el3            |$("h1,div,p")              |All `<h1>`, `<div>` and `<p>` elements|
|07.|:first                 |$("p:first")               |The first `<p>` element|
|08.|:last                  |$("p:last")                |The last `<p>` element|
|09.|:even                  |$("tr:even")               |All even `<tr>` elements|
|10.|:odd                   |$("tr:odd")                |All odd `<tr>` elements|
|11.|:first-child           |$("p:first-child")         |All `<p>` elements that are the first child of their parent|
|12.|:first-of-type         |$("p:first-of-type")       |All `<p>` elements that are the first `<p>` element of their parent|
|13.|:last-child            |$("p:last-child")          |All `<p>` elements that are the last child of their parent|
|14.|:last-of-type          |$("p:last-of-type")        |All `<p>` elements that are the last `<p>` element of their parent|
|15.|:nth-child(n)          |$("p:nth-child(2)")        |All `<p>` elements that are the 2nd child of their parent|
|16.|:nth-last-child(n)     |$("p:nth-last-child(2)")   |All `<p>` elements that are the 2nd child of their parent, counting from the last child|
|17.|:nth-of-type(n)        |$("p:nth-of-type(2)")      |All `<p>` elements that are the 2nd `<p>` element of their parent|
|18.|:nth-last-of-type(n)   |$("p:nth-last-of-type(2)") |All `<p>` elements that are the 2nd `<p>` element of their parent, counting from the last child|
|19.|:only-child            |$("p:only-child")          |All `<p>` elements that are the only child of their parent|
|20.|:only-of-type          |$("p:only-of-type")        |All `<p>` elements that are the only child, of its type, of their parent|
|21.|parent > child         |$("div > p")               |All `<p>` elements that are a direct child of a `<div>` element|
|22.|parent descendant      |$("div p")                 |All `<p>` elements that are descendants of a `<div>` element|
|23.|element + next         |$("div + p")               |The `<p>` element that are next to each `<div>` elements|
|24.|element ~ siblings     |$("div ~ p")               |All `<p>` elements that are siblings of a `<div>` element|
|25.|:eq(index)             |$("ul li:eq(3)")           |The fourth element in a list (index starts at 0)|
|26.|:gt(no)                |$("ul li:gt(3)")           |List elements with an index greater than 3|
|27.|:lt(no)                |$("ul li:lt(3)")           |List elements with an index less than 3|
|28.|:not(selector)         |$("input:not(:empty)")     |All input elements that are not empty         |
|29.|:header                |$(":header")               |All header elements `<h1>`, `<h2>` ...|
|30.|:animated              |$(":animated")             |All animated elements|
|31.|:focus                 |$(":focus")                |The element that currently has focus|
|32.|:contains(text)        |$(":contains('Hello')")    |All elements which contains the text "Hello"|
|33.|:has(selector)         |$("div:has(p)")            |All `<div>` elements that have a `<p>` element|
|34.|:empty                 |$(":empty")                |All elements that are empty|
|35.|:parent                |$(":parent")               |All elements that are a parent of another element|
|36.|:hidden                |$("p:hidden")              |All hidden `<p>` elements|
|37.|:visible               |$("table:visible")         |All visible tables|
|38.|:root                  |$(":root")                 |The document's root element|
|39.|:lang(language)        |$("p:lang(de)")            |All `<p>` elements with a lang attribute value starting with "de" |
|40.|[attribute]            |$("[href]")                |All elements with a href attribute|
|41.  |[attribute=value]      |$("[href='default.htm']")  |All elements with a href attribute value equal to "default.htm"|
|42.  |[attribute!=value]     | $("[href!='default.htm']")|All elements with a href attribute value not equal to "default.htm"|
|43.  |[attribute$=value]     |$("[href$='.jpg']")        |All elements with a href attribute value ending with ".jpg"|
|44.  |[attribute|=value]     |$("[title|='Tomorrow']")   |All elements with a title attribute value equal to 'Tomorrow', or starting with 'Tomorrow' followed by a hyphen|
|45.  |[attribute^=value]     |$("[title^='Tom']")        |All elements with a title attribute value starting with "Tom"|
|46.  |[attribute~=value]     |$("[title~='hello']")      |All elements with a title attribute value containing the specific word "hello"|
|47.  |[attribute*=value]     |$("[title*='hello']")      |All elements with a title attribute value containing the word "hello"| 
|48.|:input                 |$(":input")                |All input elements|
|49.|:text                  |$(":text")                 |All input elements with type="text"|
|50.|:password              |$(":password")             |All input elements with type="password"|
|51.|:radio                 |$(":radio")                |All input elements with type="radio"|
|52.|:checkbox              |$(":checkbox")             |All input elements with type="checkbox"|
|53.|:submit                |$(":submit")               |All input elements with type="submit"|
|54.|:reset                 |$(":reset")                |All input elements with type="reset"|
|55.|:button                |$(":button")               |All input elements with type="button"|
|56.|:image                 |$(":image")                |All input elements with type="image"|
|57.|:file                  |$(":file")                 |All input elements with type="file"|
|58.|:enabled               |$(":enabled")              |All enabled input elements|
|59.|:disabled              |$(":disabled")             |All disabled input elements|
|60.|:selected              |$(":selected")             |All selected input elements|
|61.|:checked               |$(":checked")              |All checked input elements|


#### JQUERY WITH HTML AND CSS

|Sl.No|Method                |  Description                                      |
|-----|----------------------|---------------------------------------------------|
| 01. |*addClass()           |Adds one or more class names to selected elements|
| 02. |after()               |Inserts content after selected elements|
| 03. |append()              |Inserts content at the end of selected elements|
| 04. |appendTo()            |Inserts HTML elements at the end of selected elements|
| 05. |*attr()               |Sets or returns attributes/values of selected elements|
| 06. |before()              |Inserts content before selected elements|
| 07. |clone()               |Makes a copy of selected elements|
| 08. |*css()                |Sets or returns one or more style properties for selected elements|
| 09. |closest()			 |get the first element that matches the selector|
| 10. |detach()              |Removes selected elements (keeps data and events)|
| 11. |empty()               |Removes all child nodes and content from selected elements|
| 12. |hasClass()            |Checks if any of the selected elements have a specified class name|
| 13. |height()              |Sets or returns the height of selected elements|
| 14. |*html()               |Sets or returns the content of selected elements|
| 15. |innerHeight()         |Returns the height of an element (includes padding, but not border)|
| 16. |innerWidth()          |Returns the width of an element (includes padding, but not border)|
| 17. |insertAfter()         |Inserts HTML elements after selected elements|
| 18. |insertBefore()        |Inserts HTML elements before selected elements|
| 19. |offset()              |Sets or returns the offset coordinates for selected elements (relative to the document)|
| 20. |offsetParent()        |Returns the first positioned parent element|
| 21. |outerHeight()         |Returns the height of an element (includes padding and border)|
| 22. |outerWidth()          |Returns the width of an element (includes padding and border)|
| 23. |position()            |Returns the position (relative to the parent element) of an element|
| 24. |prepend()             |Inserts content at the beginning of selected elements|
| 25. |prependTo()           |Inserts HTML elements at the beginning of selected elements|
| 26. |prop()                |Sets or returns properties/values of selected elements|
| 27. |*remove()             |Removes the selected elements (including data and events)|
| 28. |*removeAttr()         |Removes one or more attributes from selected elements|
| 29. |*removeClass()        |Removes one or more classes from selected elements|
| 30. |removeProp()          |Removes a property set by the prop() method|
| 31. |replaceAll()          |Replaces selected elements with new HTML elements|
| 32. |replaceWith()         |Replaces selected elements with new content|
| 33. |*scrollLeft()         |Sets or returns the horizontal scrollbar position of selected elements|
| 34. |*scrollTop()          |Sets or returns the vertical scrollbar position of selected elements|
| 35. |text()                |Sets or returns the text content of selected elements|
| 36. |toggleClass()         |Toggles between adding/removing one or more classes from selected elements|
| 37. |unwrap()              |Removes the parent element of the selected elements|
| 38. |*val()                |Sets or returns the value attribute of the selected elements (for form elements)|
| 39. |width()               |Sets or returns the width of selected elements|
| 40. |wrap()                |Wraps HTML element(s) around each selected element|
| 41. |wrapAll()             |Wraps HTML element(s) around all selected elements|
| 42. |wrapInner()           |Wraps HTML element(s) around the content of each selected element|
