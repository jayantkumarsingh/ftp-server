# Simple ftp server


## How to install:

```
cd to the ftp dir
make
execute with ./myftp
```

## Commands that are currently implemented:

* USER PASS - anonymous ftp only at the moment
* PASV PORT LIST CWD PWD MKD RMD RETR STOR DELE SIZE ABOR QUIT TYPE QUOTE SITE NOOP
* Custom ftp commands

### TODO
* user log in
* get file
* put file
* mkdir, rm, rmdir, CHMOD

Server currently works with linux only because of splice() and sendfile() functions.
It should be easy enough to implement RETR and STOR for other systems too, so it is
in my todo list.

This server currently doesn't support ASCII mode but this sould not be a
problem with any modern system or ftp client.
