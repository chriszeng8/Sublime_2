### Snippet

Very quick way to auto-complete syntax, by typing part of syntax, and then press tab.

To open snippet, Tools -> Snippet

Command + Control + P, and type snippet, to see all snippets associated with the type of file opened.

Snippet is associate with syntax type, if syntax is set as html, the snippet will be different after the syntax is set as javascript.


For example, change the syntax to javascript by pressing ```Ctrl + Command + P```, then enter ```js```.
See Snippet if by Ctrl + Command + P, then enter ```Snippet: if```, or ```sni if``` for short fuzzy search. Alternatively, just type in ```if``` and press tab, to autocomplete.
```ife``` for if else. ```fun``` followed by tab, for ```function function_name (argument) {
	// body...
}```


### Customized Snippet

Go to ```Tools``` -> ```New Snippet...``` to create new custom snippet.
The default template is:
```
<snippet>
	<content><![CDATA[
Hello, ${1:this} is a ${2:snippet}.
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<!-- <tabTrigger>hello</tabTrigger> -->
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>
```

The ```${#}``` curve is the default parameter(s) highlighted when snippets get created.
uncomment the tabTrigger tab by ```Command + /``` to autocomplete by tab

save the file as ```hello.sublime-snippet``` in the User folder (I created a JavaScript folder within the User folder to store all snippets associated with JavaScript, creating a folder to allocate snippets associated with one syntax is a good practice.)

####Example 1: IIFE
Another working example, create our own immediately invoked function express (IIFE):

```
(function (argument) {
	// body...
})();
```
We just need to save the following snippet as ```iife.sublime-snippet``` in Package/User/JavaScript folder.
```
<snippet>
	<content><![CDATA[
(function () {
	${1}
})();
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>iife</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>
```

####Example 2: Backbone model extend
```
Backbone.Model.extend({
	//body
});
```

We create an folder within the javascript called Backbone, and store the following code
as ```model-extend.sublime-snippet``` in the ```Package\User\JavaScript\Backbone``` folder.

```
<snippet>
	<content><![CDATA[
Backbone.Model.extend({
	${1}
});
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>bm</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>
```