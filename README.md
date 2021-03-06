# Simple Logging
Just some simple logging functions that can be used in pretty much any program.

## Installation
This program was developed and tested in [`python 3.10`](https://docs.python.org/3/index.html) and uses standard libraries. Although many earlier versions will work, I just haven't bothered testing them.

You can install this library with the following command
```
pip install Simple-Logger-Tool -U
```

## Usage
Import the logger class into your python file with the code below.
```
from Simple_Logger_Tool.Simple_Logger_Tool import Logger
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
MIT License

Copyright (c) 2022 Matt

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.