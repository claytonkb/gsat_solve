gsat_solve
==========

A simple GSAT-based SAT-solver. Use command-code 3 to load a standard DIMACS-
format CNF file. Solve with command-code 4 (optionally specify number of
tries and number of flips per try). Dump result to screen with command-code
5. Dump to file with command-code 6 (be sure to create work directory first).

Building
--------

This program is dependent on three other libararies in my repository. Here is
a sample build procedure:

    % git clone https://github.com/claytonkb/lib_babel
    % git clone https://github.com/claytonkb/cnf_parse
    % git clone https://github.com/claytonkb/sat_tools
    % git clone https://github.com/claytonkb/gsat_solve
    % cd gsat_solve
    % perl make.pl
    % bin/test

If you want verbosity during the build, provide the -v or -V switch to make.pl.
If you want to write your own Makefile or use another build solution, use the
-vt option (verbose, testing-only) to see the shell commands that make.pl would
issue if it were run without the -t switch to aid you in constructing your own
build solution.

