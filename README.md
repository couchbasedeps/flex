Couchbasedeps Flex
------------------

*Linux/MacOS*

Due to autotools and git disagreeing about the importance of timestamps,
it's not really possible to check out a "release" version of flex
from git. On the other hand, building flex from a non-"release" package
requires far more tools on the build slave. So, as a compromise, and
since the source is quite small, we simply check in the tar.gz of
the "release" source code, bypassing git.

*Windows*

It's extremely difficult to build flex at all on Windows, so we simply
commit a released binary from the gnuwin32 project. The win\_flex\_bison
project is better supported and more up-to-date, but the users of flex
in the company preferred the gnuwin32 form for now, so here it is.
