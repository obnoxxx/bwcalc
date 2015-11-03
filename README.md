# bwcalc - a bandwidth/size/time calculator

Version 0.2 2004-10-12

Copyright (C) Michael Adam <obnox@samba.org> 2004,2015

License: GPLv3+

USAGE: bwcalc [-s <size>] [-t <time>] [-b <bw>] [-o <unit>] [-p <num>] [-l]

  One or two of the three input options -s, -b, -t can be given.
  If only one is given, then the given value is transferred into
  the desired output unit. If two are given, then the third entity
  is the target of the calculation.

  Input options format:

  - Bandwidth: <number>[<unit>]  ("/sec" is omitted)
  - Size:      <number>[<unit>]
  - Time:      <number>[smhdw]?

  The optional unit for bandwidth and size is of the form
  [<prefix>][<base>] where prefix is one of K, Ki, M, Mi, G, Gi, T, Ti
  and <base> can be "b" for bit and "B" for byte. The default
  base unit is "b" for bandwidth and "B" for size.

  The ouptut unit for size and bandwidth target can be given
  with the the -o options in the same way as for the input options.
  The default for the base unit is bit for bandwidth target and
  bytes for size target.

  The precision for rounding output can be given with the "-p" switch.

  Long output format can be chosen with the "-l" switch.

