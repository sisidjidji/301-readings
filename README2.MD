# READ2

## 1. What is JQUERY:
jQuery is a javaScript file that you include in your web pages.it let you find element using CSS-style selectors and then do something with the elements using jQuery methods.



## 2. Syntax:

|Syntax	|Description|	
|-------|-----------|
|$("*")	|Selects all elements|
|$(this)|Selects the current HTML element|
|$("p.intro")|	Selects all < p> elements with class="intro"|
|$("p:first")|	Selects the first < p> element|
|$("ul li:first")|Selects the first < li> element of the first < ul>|	
|$("ul li:first-child")|	Selects the first < i> element of every < ul>|	
|$("[ href]")	Selects all| elements with an href attribute|
|$("a[ target='_blank']")	|Selects all < a> elements with a target attribute value equal to "_blank"|	
|$("a[ target!='_blank']")|	Selects all < a> elements with a target attribute value NOT equal to "_blank"|	
|$(":button")|	Selects all < button> elements and < input> elements of type="button"|
|$("tr:even")|	Selects all even < tr> elements|
|$("tr:odd")|Selects all odd < tr> elements|

## 3. jQuery Methods :

jQuery provides various methods for different tasks e.g. manipulate DOM, events etc. The following table lists exemples and categories of methods.

|Category| Methods|
|--------|--------|
|DOM Manipulation|after(),append(),attr(),before(),|
|Traversing|children(),closest(),each(),first(),next(),filter()|
|CSS|addClass(),css(),hasClass(),removeClass(),toggleClass()|
|Attributes|attr(),html(),removeAttr(),prop(),val(),|
|Events|bind(),blur(),change(),click(),dblclick(),focus(),|
|Dimensions|height(),width(),innerHeight(),innerWidth(),|