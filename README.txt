This is the implementation which is used to EXPLAIN the
submission. It is NOT meant to be optimized in any way
really.

Please ensure commenting is good

Many files are virtually identical to those in the 
Optimized directory. Identical ones are not replicated
via sym-links as I suspect these will break NIST/Windows/SVN
and other things. So doing this the hard way.

Type
  make
to compile. It assumes that KECCAK stuff has already
been compiled

Test-SubRoutines.c
  - Produces some KAT files for testing
  - Tests other data

Time-Solution.c
  - Does some naive timing

The directory
  NIST
contains the files to produce the main KAT files according
to the NIST api. Just go into this directory and type
  make
Then compare the KAT files in the subdirectory
  NIST/KAT-Test
with those files which can be found in  
  ../KAT

