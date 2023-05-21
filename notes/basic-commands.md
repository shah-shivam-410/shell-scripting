# Basic commads in linux

## ECHO command
Prints or returns any text passed as argument for echo command.

### Basic use with quotes

Suppose var1="Abc"

    echo "Hello world $var1" -> Hello world Abc
    echo 'Hello world $var1' -> Hello world $var1
    echo `date` -> Sun, May 21, 2023  3:12:03 PM

### Options

* -e : To evalualate baslash characters in echo string

* -n : To skip trailling new line

## READ command

Used to take input from user from interactive terminal.

`read -r -p "Please provide filename:"`

### Options

The read command takes the following options:

* -a array Store the words in an indexed array named array. Numbering of array elements starts at zero.
* -d delim Set the delimiter character to delim. This character signals the end of the line. If -d is not used, the default line delimiter is a newline.
* -e Get a line of input from an interactive shell.
* -n nchars Read only nchars characters rather than waiting for a complete line of input.
* -p prompt Display prompt on standard error, without a trailing newline, before attempting to read any input. The prompt is displayed only if input is coming from a terminal.
* -r Do not allow backslashes to escape any characters.
* -s Do not echo input coming from a terminal.
* -t timeout Cause read to time out and return failure if a complete line of input is not read within timeout seconds. timeout may be a decimal number with a fractional portion following the decimal point. This option is only effective if read is reading input from a terminal, pipe, or other special file; it has no effect when reading from regular files. If timeout is 0, read returns immediately, without trying to read any data. The exit status is 0 if input is available on the specified file descriptor, non-zero otherwise. The exit status is greater than 128 if the timeout is exceeded.
* -u fd Read input from file descriptor fd.