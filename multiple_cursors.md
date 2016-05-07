##Multiple Cursors
####Command + D

Useful Application:
Change a variable throughout a file.


Instead of using find and replace (Command + Shift + F), enable Multiple Cursors:
```Command + D``` will select the selected variable along with the next selection.
keep pressing command + D multiple times to increment the number of selection


```
AList = {}
AList['a'] = 1
AList['b'] = 2
```

so moving the cursor anywhere along the var AList and press ```Command + D``` once will highlight the selected variable, press again twice will select three of the AList variables.


####Control + Command + G

will select all occurrences of the selected word.


####Alt

To enable column selection, hold ```alt``` and select columns