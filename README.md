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
Worked: 00:00:04
```
the script looks for the 'stop' string and then calculates the time difference from the last logged entry
the log is saved to a file named 'log-YYYY-MM-DD'
when the stop command is used, the time worked is output to the console as well as the log file
