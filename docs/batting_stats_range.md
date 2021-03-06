# batting_stats_range

__batting_stats_range(start_dt, end_dt=None)__

The batting_stats_range function returns batting stats from Baseball Reference, aggregated over a user-defined time range.

## Arguments
__start_dt:__ String. The beginning of the date range you want batting stats for. Format: "YYYY-MM-DD". 

__end_dt:__ String. The end of the date range you want batting stats for. If omitted, the funciton will return only data from the start_dt. Format: "YYYY-MM-DD".

## Examples of valid queries

~~~~
from pybaseball import batting_stats_range

# retrieve all players' batting stats for the month of May, 2017 
data = batting_stats_range("2017-05-01", "2017-05-28")

# retrieve batting stats for only August 24, 2016
data = batting_stats_range("2016-08-24",)
~~~~
