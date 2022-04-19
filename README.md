# Simple Logging
Just some simple logging functions that can be used in pretty much any program.

## Installation
This program was developed and tested in `python 3.10` and uses standard libraries. Although many earlier versions will work, I just haven't bothered testing them.

## Usage
Simply download the [Simple_Logger.py](Simple_Logger.py) file and import the logger class into your python file with the code below.
```
from Simple_Logger import Logger
```

You can create a logger object by using the code below. Where I have put test logger, you can put whatever you want the logger to be called on your system. <br>

One suggested usage would be today's date. This name is used to name the file it stores the logs to. This means that if you provide an already used name then it will append to that log file.
```
lgr = Logger("Test_Logger")
```
This code is an example of logging something for information
```
lgr.log_info("This is a test of the logging info")
```
This code is an example of logging something for warnings
```
lgr.log_warning("This is a test of the logging warning")
```
This code is an example of logging something for errors
```
lgr.log_error("This is a test of the logging error")
```
An example output of the code above in the log (txt) file is:<br>
```
###############################################################
[19/04/2022 at 16:29:11]
[LOGGER INITIALIZED]
###############################################################
[19/04/2022 at 16:29:11 | INFO   ]: This is a test of the logging info
[19/04/2022 at 16:29:11 | WARNING]: This is a test of the logging warning
[19/04/2022 at 16:29:11 | ERROR  ]: This is a test of the logging error
```

## License
[See license file](LICENSE)