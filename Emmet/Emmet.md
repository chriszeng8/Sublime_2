
Emmet is for fast HTMl editing
First install package, and search for Emmet.

First: set Syntax to HTML (remember, our best friend: Command + Ctrl + P :) )
e.g., 
The following HTML can be created by:
```
<ul>
	<li></li>
	<li></li>
	<li></li>
</ul>
```

can be created by typing ```ul>li*3``` followed by hitting a tab.

Another example:
A container div containg three different divs.
```
<div class="container">
	<div class="header"></div>
	<div class="main"></div>
	<div class="footer"></div>
</div>
```
can be created by
```
.container>.header+.main+.footer
```
followed by pressing tab.


1. creating a div.

If no tag name is specified, a div is assumed to be tag type.
```.header```
and ```div.header``` are the same.

2. plus (+) to create siblings
3. > is to create children.
```.header+.footer``` gives
```
<div class="header"></div>
<div class="footer"></div>
```
4. user HTML tag instead of div tag.
```head```
gives
```
<head></head>
```
instead of ```.head```
<div class="head"></div>

5. div syntax is same as CSS (. is class, # is id)
4. * for multiple elements
```ul*3```
give
```
<ul></ul>
<ul></ul>
<ul></ul>
```

6. anchor with class, or id
```a.button``` gives
```
<a href="" class="button"></a>
```

anchor with url
```a[href=www.google.com]```
gives
```
<a href="www.google.com"></a>
```
note that quotation is not even required.

7. {} fill in value within element
```li{a}+li{b}```
gives
```
<li>a</li>
<li>b</li>
```

e.g., 
```li{hello world}*2``` gives
```
<li>hello world</li>
<li>hello world</li>
```

e.g., 
```
ul>li*2>a[href=#]{Some Link}
```
gives
```
<ul>
	<li><a href="#">Some Link</a></li>
	<li><a href="#">Some Link</a></li>
</ul>
```

Sublime can auto wrap a variable with () by highligh the selected variables/line, then enter open bracket (.

An example with more hierachy:
```
.continer>(.header>header>h1{My Website})+.main+.footer>footer
```
```
<div class="continer">
	<div class="header">
		<header>
			<h1>My Website</h1>
		</header>
	</div>
	<div class="main"></div>
	<div class="footer">
		<footer></footer>
	</div>
</div>

```
Command + L to select the whole line