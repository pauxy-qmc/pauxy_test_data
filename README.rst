Repository for longer and parallel tests of pauxy. Avoid storing potentially large files in the main repo.

Note short tests are determininistic and not meant to be statistically meaningful.

Require testcode to run tests. https://github.com/jsspencer/testcode

To run MPI tests do the following:

::

    python /path/to/testcode/bin/testcode.py -v  -e /path/to/bin/pauxy run --user-option=pauxy launch_parallel 'mpiexec -np tc.nprocs python -u'
