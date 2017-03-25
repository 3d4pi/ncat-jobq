# ncat-jobq
```
NAME
       ncat-jobq - Serve queue contents to network clients using ncat

SYNOPSIS
       ncat-jobq -q <filename> [OPTION]...

DESCRIPTION
       Pop and send the first line of a file to network clients.
       When the file is empty, send an empty string.
       One client at a time. You can specify the local server address and port.
       Append one line per incoming transaction to ${QUEUE}.log

OPTIONS
       -h, --help
              this text

       -q, --queue
              The file containing the queue (WILL BE EMPTIED)

       -l, --local <addr>
              Local ip address to bind to, defaults to 0.0.0.0

       -p, --port <port>
              Local tcp port number, defaults to 3354

       -o, --options <string>
               Additional ncat options
```
