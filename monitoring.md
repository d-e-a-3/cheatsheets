## OS X

Command | Description
------- | -----------
**`top -o cpu`** | Sort by CPU usage
**`iosnoop`** | Traces disk I/O execution live
**`errinfo`** | Summary of which system calls are failing
**`opensnoop`** | Traces file opens and prints various details
**`dtruss`** | Linus strace equivalent
**`dtruss -e`** | Print elapsed times. Useful to find bottlenecks
**`dtruss -d`** | Print relatice times. Useful when output order is important (output can be shuffled slightly due to CPU buffering on multi-CPU systems)
