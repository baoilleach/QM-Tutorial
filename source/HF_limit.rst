Effect of basis set
===================

We are going to compare the effects of the basis set on the energy of a RHF calculation on water.

Running GAMESS
--------------

To speed things up, we are going to use the geometry we found for RHF/3-21G and use that for our calculations.

In Avogadro, open the output file from the RHF/3-21G geometry optimisation of water (remember to rename the file to :file:`.gamout`), and create several input files for a single-point RHF calculations with increasing basis set size.

The notation for calculations of this type uses the ``//`` notation; for example, ``RHF/6-31G//RHF/3-21G``.

When they have all been created, run each of them in turn.

(Note to self: Is there time to run an MP2/3-21G calculation?)

Analyse
-------

For each calculation, note the final RHF energy and also the wall clock time (found at the end of the output file).

Q. What is the effect of the basis set size on the energy? Based on this, does it make sense to compare the results of calculations with different basis set sizes?

Q. What is the effect of the basis set size on the computation speed?
