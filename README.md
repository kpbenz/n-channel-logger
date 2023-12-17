# n-channel-logger

## Features
- Configurable number of space-separated data fields logged
- Adds ISO timestamps (2023-12-01T14:50:00UTC) in second precision
- Optional CRC32 checksum
- Daily rotation of logfiles

## Call

n-channel-logger [-c] [-n \<name-prefix\>] [-d \<data-directory\>] \<device\>
