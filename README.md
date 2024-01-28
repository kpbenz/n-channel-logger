# n-channel-logger

## Features
- Log data strings
- Option: Adds ISO timestamps (2023-12-01T14:50:00.012+13:00) in millisecond precision with timezone offset
- Option: Check CRC-16 at end of record and mark record as failed in case of mismatch.
- Daily rotation of logfiles

## Call

n-channel-logger [-c] [-t] [-n \<name-prefix\>] [-d \<data-directory\>] \<device\>
