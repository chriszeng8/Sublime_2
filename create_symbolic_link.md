Sublime text can be open from terminal by creating a symbolic link, similar to alias.

```ln -s "/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl" /bin/subl```

If it says permission denied, go 

```sudo !!```

as ```!!``` repeat the previous command executed.

Restart the terminal, and can type in ```subl``` followed by the folder or file name.