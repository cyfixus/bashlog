# bashlog
Simple logging tool for bash shell

## usage
enable the file to be executed 
```
chmod u+x log
```

execute the file with the first argument being 'start' or 'stop'
```
./log start developing log readme
./log stop
```
the script looks for the 'stop' string and then calculates the time difference from the last logged entry
