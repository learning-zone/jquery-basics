## jQuery functions 


#### jQuery Selectors


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


#### jQuery with HTML & CSS

|Sl.No|Method                |  Description                                      |
|-----|----------------------|---------------------------------------------------|
| 01. |addClass()           |Adds one or more class names to selected elements|
| 02. |after()               |Inserts content after selected elements|
| 03. |append()              |Inserts content at the end of selected elements|
| 04. |appendTo()            |Inserts HTML elements at the end of selected elements|
| 05. |attr()               |Sets or returns attributes/values of selected elements|
| 06. |before()              |Inserts content before selected elements|
| 07. |clone()               |Makes a copy of selected elements|
| 08. |css()                |Sets or returns one or more style properties for selected elements|
| 09. |closest()			 |get the first element that matches the selector|
| 10. |detach()              |Removes selected elements (keeps data and events)|
| 11. |empty()               |Removes all child nodes and content from selected elements|
| 12. |hasClass()            |Checks if any of the selected elements have a specified class name|
| 13. |height()              |Sets or returns the height of selected elements|
| 14. |html()               |Sets or returns the content of selected elements|
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
| 27. |remove()             |Removes the selected elements (including data and events)|
| 28. |removeAttr()         |Removes one or more attributes from selected elements|
| 29. |removeClass()        |Removes one or more classes from selected elements|
| 30. |removeProp()          |Removes a property set by the prop() method|
| 31. |replaceAll()          |Replaces selected elements with new HTML elements|
| 32. |replaceWith()         |Replaces selected elements with new content|
| 33. |scrollLeft()         |Sets or returns the horizontal scrollbar position of selected elements|
| 34. |scrollTop()          |Sets or returns the vertical scrollbar position of selected elements|
| 35. |text()                |Sets or returns the text content of selected elements|
| 36. |toggleClass()         |Toggles between adding/removing one or more classes from selected elements|
| 37. |unwrap()              |Removes the parent element of the selected elements|
| 38. |val()                |Sets or returns the value attribute of the selected elements (for form elements)|
| 39. |width()               |Sets or returns the width of selected elements|
| 40. |wrap()                |Wraps HTML element(s) around each selected element|
| 41. |wrapAll()             |Wraps HTML element(s) around all selected elements|
| 42. |wrapInner()           |Wraps HTML element(s) around the content of each selected element|


#### jQuery Events

|Sl.No|Method                |  Description                                      |
|-----|----------------------|---------------------------------------------------|
| 01. |bind()                |Attaches event handlers to elements|
| 02. |blur()                |Attaches/Triggers the blur event|
| 03. |change()              |Attaches/Triggers the change event|
| 04. |click()               |Attaches/Triggers the click event|
| 05. |dblclick()            |Attaches/Triggers the double click event|
| 06. |delegate()            |Attaches a handler to current, or future, specified child elements of the matching elements|
| 07. |event.currentTarget   |The current DOM element within the event bubbling phase|
| 08. |event.data            |Contains the optional data passed to an event method when the current executing handler is bound|
| 09. |event.delegateTarget   |Returns the element where the currently-called jQuery event handler was attached|
| 10. |event.isDefaultPrevented() |Returns whether event.preventDefault() was called for the event object|
| 11. |event.isImmediatePropagationStopped()| Returns whether event.stopImmediatePropagation() was called for the event object|
| 12. |event.isPropagationStopped() |Returns whether event.stopPropagation() was called for the event object|
| 13. |event.namespace              |Returns the namespace specified when the event was triggered|
| 14. |event.pageX                  |Returns the mouse position relative to the left edge of the document|
| 15. |event.pageY                  |Returns the mouse position relative to the top edge of the document|
| 16. |event.preventDefault()       |Prevents the default action of the event|
| 17. |event.relatedTarget          |Returns which element being entered or exited on mouse movement.|
| 18. |event.result                 |Contains the last/previous value returned by an event handler triggered by the specified |event|
| 19. |event.stopImmediatePropagation() |Prevents other event handlers from being called|
| 20. |event.stopPropagation()          |Prevents the event from bubbling up the DOM tree, preventing any parent handlers from being notified of the event|
| 21. |event.target          |Returns which DOM element triggered the event|
| 22. |event.timeStamp       |Returns the number of milliseconds since January 1, 1970, when the event is triggered|
| 23. |event.type            |Returns which event type was triggered|
| 24. |event.which           |Returns which keyboard key or mouse button was pressed for the event|
| 25. |focus()               |Attaches/Triggers the focus event|
| 26. |focusin()             |Attaches an event handler to the focusin event|
| 27. |focusout()            |Attaches an event handler to the focusout event|
| 28. |hover()               |Attaches two event handlers to the hover event|
| 29. |keydown()             |Attaches/Triggers the keydown event|
| 30. |keypress()            |Attaches/Triggers the keypress event|
| 31. |keyup()               |Attaches/Triggers the keyup event|
| 32. |mousedown()           |Attaches/Triggers the mousedown event|
| 33. |mouseenter()          |Attaches/Triggers the mouseenter event|
| 34. |mouseleave()          |Attaches/Triggers the mouseleave event|
| 35. |mousemove()           |Attaches/Triggers the mousemove event|
| 36. |mouseout()            |Attaches/Triggers the mouseout event|
| 37. |mouseover()           |Attaches/Triggers the mouseover event|
| 38. |mouseup()             |Attaches/Triggers the mouseup event|
| 39. |off()                 |Removes event handlers attached with the on() method|
| 40. |on()                  |Attaches event handlers to elements|
| 41  |one()                 |Adds one or more event handlers to selected elements. This handler can only be triggered once per element|
| 42. |$.proxy()             |Takes an existing function and returns a new one with a particular context|
| 43. |ready()               |Specifies a function to execute when the DOM is fully loaded|
| 44. |resize()              |Attaches/Triggers the resize event|
| 45. |scroll()              |Attaches/Triggers the scroll event|
| 46. |select()              |Attaches/Triggers the select event|
| 47. |submit()              |Attaches/Triggers the submit event|
| 48. |trigger()             |Triggers all events bound to the selected elements|
| 49. |triggerHandler()      |Triggers all functions bound to a specified event for the selected elements|
| 50. |unbind()              |Removes an added event handler from selected elements|
| 51. |undelegate()          |Removes an event handler to selected elements, now or in the future|


#### jQuery Effetcs

|Sl.No|Method                |  Description                                      |
|-----|----------------------|---------------------------------------------------|
| 01. |animate()             |Runs a custom animation on the selected elements|
| 02. |clearQueue()          |Removes all remaining queued functions from the selected elements|
| 03. |delay()               |Sets a delay for all queued functions on the selected elements|
| 04. |dequeue()             |Removes the next function from the queue, and then executes the function|
| 05. |fadeIn()              |Fades in the selected elements|
| 06. |fadeOut()             |Fades out the selected elements|
| 07. |fadeTo()              |Fades in/out the selected elements to a given opacity|
| 08. |fadeToggle()          |Toggles between the fadeIn() and fadeOut() methods|
| 09. |finish()              |Stops, removes and completes all queued animations for the selected elements|
| 10. |hide()                |Hides the selected elements|
| 11. |queue()               |Shows the queued functions on the selected elements|
| 12. |show()                |Shows the selected elements|
| 13. |slideDown()           |Slides-down (shows) the selected elements|
| 14. |slideToggle()         |Toggles between the slideUp() and slideDown() methods|
| 15. |slideUp()             |Slides-up (hides) the selected elements|
| 16. |stop()                |Stops the currently running animation for the selected elements|
| 17. |toggle()              |Toggles between the hide() and show() methods|


#### jQuery Ajax

|Sl.No|Method                |  Description                                      |
|-----|----------------------|---------------------------------------------------|
| 01. |$.ajax()              |Performs an async AJAX request|
| 02. |$.ajaxPrefilter()     |Handle custom Ajax options or modify existing options before each request is sent and before |they are processed by $.ajax()|
| 03. |$.ajaxSetup()         |Sets the default values for future AJAX requests|
| 04. |$.ajaxTransport()     |Creates an object that handles the actual transmission of Ajax data|
| 05. |$.get()               |Loads data from a server using an AJAX HTTP GET request|
| 06. |$.getJSON()           |Loads JSON-encoded data from a server using a HTTP GET request|
| 07. |$.getScript()         |Loads (and executes) a JavaScript from a server using an AJAX HTTP GET request|
| 08. |$.param()             |Creates a serialized representation of an array or object (can be used as URL query string for AJAX requests)|
| 09. |$.post()              |Loads data from a server using an AJAX HTTP POST request|
| 10. |ajaxComplete()        |Specifies a function to run when the AJAX request completes|
| 11. |ajaxError()           |Specifies a function to run when the AJAX request completes with an error|
| 12. |ajaxSend()            |Specifies a function to run before the AJAX request is sent|
| 13. |ajaxStart()           |Specifies a function to run when the first AJAX request begins|
| 14. |ajaxStop()            |Specifies a function to run when all AJAX requests have completed|
| 15. |ajaxSuccess()         |Specifies a function to run when an AJAX request completes successfully|
| 16. |load()                |Loads data from a server and puts the returned data into the selected element|
| 17. |serialize()           |Encodes a set of form elements as a string for submission|
| 18. |serializeArray()      |Encodes a set of form elements as an array of names and values|
