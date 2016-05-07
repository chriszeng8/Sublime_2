##Enabling opening project with Sublime from right clicking Folder

###(Mac Specific)

Open Automator:

* Add Service
* Set Variables as: Run Shell Script
* Paste the following command in (Shell: /bin/zsh)

/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl -n $@

Change Service receives selected to:

```files or folders```

Save now, and save it as:
```Open-in-Sublime```


Now right click an folder, and go to services, click Open-in-Sublimem and voila. you can now open the whole project with sublime text. 