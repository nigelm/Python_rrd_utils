# Python RRD Utils

This is a rework of some existing python utilities for working with RRDs to
make them work with python3.  Otherwise minimal changes have been made.

The utilities are:-

- `rrdinfo-parser.py` - https://github.com/tksunw/python-rrd-schema-parse
  Retrieve the rrdcreate parameters from an existing RRD file.

- `merge-rrd.py` - retrieved from https://oss.oetiker.ch/rrdtool/pub/contrib/
  Merge some RRD files.  Original README:-

```
Usage: merge-rrd.py <old rrd> <new rrd> <merged rrd>

merge-rrd.py is a python script that merges that data found in rrd
files.  This assumes that the two rrds are have the same data structure.

The script creates the merged rrd by copying the entries from the new rrd.
If the new rrd has database entries with missing data, then the records
of the old rrd are used instead.  This mean that data from the new rrd
will always take precedence over the data in the old rrd.

Please report any bug at:
 minhong.tsai@gmail.com                                    4-11-2005
```
