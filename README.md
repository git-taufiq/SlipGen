#SlipGen
-----------

Hybrid *k*<sup>-2</sup> hybrid slip generator

The repository contains the main Fortran code and an example input file. I hope they both are self-explanatory, 
but do not hesitate to contact me if you have any questions or meet any problems with
running the code.

###Brief description of the I/O files

####Input:
 - `slipgen.in`: fault model definition

####Output:
 - `slipgen.txt`: generated hybrid slip distribution
 - `slipx.txt` and `slipy.txt`: slices of the slip distribution
 - `specx.txt` and `specy.txt`: slices of the slip Fourier spectrum

###Note on compiling:

Some compilers may produce error when compiling. Most likely it will be due to the use an old Fortran trick,
where complex arrays are passed to a subroutine that expects a real array.
This can be solved by using an appropriate switch. In Intel Fortran compiler in Microsoft Visual Studio do the following.
Right-click on your project in the right-hand-side window ("Solution explorer") and select
Properties. Select Fortra/Diagnostics in the dialog and change the option "Check routine interfaces" to No.

###References
 - Gallovič, F., and J. Brokešová (2004). On strong ground motion synthesis with k^-2 slip distributions, J. Seismology, 8, 211-224.
 - Gallovič, F., and J. Brokešová (2004). The k^-2 rupture model parametric study: example of the 1999 Athens earthquake, Studia geoph. et geod., 48, 589-613.
 - See also http://geo.mff.cuni.cz/~gallovic/.
