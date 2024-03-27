Tradelog is a Shell script designed for analyzing trading logs on the stock exchange. It can perform various operations on logs and provides users with useful information about trading transactions.

#### Usage:
```bash
./tradelog.sh [-h|--help] [FILTER] [COMMAND] [LOG [LOG2 [...]]]
```

#### Filters:
- `-a DATETIME`: Displays only records after the specified date and time.
- `-b DATETIME`: Displays only records before the specified date and time.
- `-t TICKER`: Displays only records corresponding to the given ticker.
- `-w WIDTH`: Sets the width of the graphs.

#### Commands:
- `list-tick`: Lists the stock symbols (tickers).
- `profit`: Displays the total profit from closed positions.
- `pos`: Displays the values of currently held positions, sorted in descending order of value.
- `last-price`: Displays the last known price for each ticker.
- `hist-ord`: Displays a histogram of transaction counts by ticker.
- `graph-pos`: Displays a graph of position values by ticker.

#### Help:
- `-h`, `--help`: Displays help with a brief description of each command and filter.

### Installation:
To run the script, you need to have a shell (bash) installed and the relevant trading logs from the stock exchange.

### Execution:
```bash
./tradelog.sh [OPTIONS] [LOG_FILE]
```

#### Example:
```bash
./tradelog.sh -a "2023-01-01 00:00:00" -b "2023-12-31 23:59:59" -t "AAPL" -w 80 -h log_file.csv.gz
```
