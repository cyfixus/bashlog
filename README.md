# bashlog
Simple logging tool for bash shell

## usage
enable the file to be executed 
```
chmod u+x log
```

execute the file with the first argument being 'start', 'stop', or 'check'
```
./log start developing log readme
start   >> 2019-06-03 22:09:17 : developing readme

$ ./log check
start   >> 2019-06-03 22:10:38 : developing readme
Worked: 00:00:06

$ ./log stop developing readme
stop    >> 2019-06-03 22:11:04 : developing readme
Worked: 00:00:26
```
the script looks for the 'stop' or 'check' string and then calculates the time difference from the last logged entry
the log is saved to a file named 'log-YYYY-MM-DD'
when the stop command is used, the time worked is output to the console as well as the log file
