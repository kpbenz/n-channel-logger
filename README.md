# n-channel-logger

## Features
- Log data strings
- Option: Adds ISO timestamps (2023-12-01T14:50:00.012+13:00) in millisecond precision and timezone offset
- Option: Check CRC-16 at end of record and mark record as failed in case of mismatch.
- Daily rotation of logfiles
- A serial devices will be opened wit 9600Bd, 8 data bits, no parity and 1 stop-bit.
- The device name '-' (dash) opens standard input instead of a serial device.

## Call

usage: n-channel-logger [-h] [-d DIRECTORY] [-p PREFIX] [-t] [-c] [-f] [-v] device

Logs a string of whitespace-separated data fields into timestamped logfiles.

### Positional arguments:
| Argument | Description |
| -------- | ----------- |
| device   | Data source |

### Pptions:
  | Short option | Long Option           | Description                                |
  | ------------ | --------------------- | ------------------------------------------ |
  | -h           | --help                | Show this help message and exit            |
  | -d DIRECTORY | --directory DIRECTORY | Target directory for logfiles              |
  | -p PREFIX,   | --prefix PREFIX       | Prefix for log files                       |
  | -t           | --time-stamping       | Prepend per-second timestamp in ISO format |
  | -c           | --crc16-verification  | Verifies the CRC-16 at end of record       |
  | -f           | --flush               | Flushes logs after every write             |
  | -v           | --verbose             | Print received strings to stdout           |
  | -V           | --version             | Show version number                        |

(c) 2023-2024 karsten@benz-engineering.co.nz
