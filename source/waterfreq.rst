Vibrational frequencies of water
================================

Vibrational frequency calculations should always be carried out to verify that a geometry optimisation has found a true minimum, and not just a saddle point.

They are also useful in their own right to find and visualise the normal modes of vibration.

Create the GAMESS input file and run GAMESS
-------------------------------------------

The vibrational frequencies are only valid at an optimised geometry so we need to use the geometry obtained in the previous calculation.

To open a GAMESS output file in Avogadro, we need to first rename it from :file:`.out` to :file:`.gamout`. Once this is done, use File/Open in Avogadro to open the file.

Next click Extensions/GAMESS/"Input Generator" and choose "Frequencies" under Calculate. Click on :guilabel:`Generate` and save the GAMESS input file.

Run GAMESS using drag-and-drop as before.

Analyse the frequencies
-----------------------

It is worth opening the GAMESS output file in Wordpad and taking a look at the NORMAL COORDINATE ANALYSIS section (see below). (Hint: In Wordpad, it is useful to "Select All" and change the font size to 8 pt.)

Q. Is this molecule at a true geometry minimum?

Q. How many frequencies are expected for a 3-atom non-linear molecule? (Hint: 3N-6)

Q. How many frequencies are present in the file? How can you account for the difference?

::

                  --------------------------------------------------------
                  NORMAL COORDINATE ANALYSIS IN THE HARMONIC APPROXIMATION
                  --------------------------------------------------------

                  ATOMIC WEIGHTS (AMU)

            1     O                15.99491
            2     H                 1.00782
            3     H                 1.00782

         MODES 1 TO 6 ARE TAKEN AS ROTATIONS AND TRANSLATIONS.

         ANALYZING SYMMETRY OF NORMAL MODES...

             FREQUENCIES IN CM**-1, IR INTENSITIES IN DEBYE**2/AMU-ANGSTROM**2,
             REDUCED MASSES IN AMU.

                                  1           2           3           4           5
               FREQUENCY:         1.33        0.16        0.00        0.33        6.17  
                SYMMETRY:         A           A           A           A           A   
            REDUCED MASS:      1.01401     6.22305     6.00353    12.81051     1.03666
            IR INTENSITY:      8.39984     0.00224     0.00000     0.52570     3.14657

          1   O            X -0.00000000 -0.04742972  0.23101688 -0.00000000  0.03749320
                           Y -0.00000000  0.23166471  0.04641338 -0.00000000 -0.02121402
                           Z -0.02017373  0.00000000  0.00000000  0.24794115 -0.00000000
          2   H            X -0.00000000 -0.04712588  0.23101681 -0.00000000  0.02610283
                           Y  0.00000000  0.21251345  0.04641346 -0.00000000  0.69693540
                           Z  0.87470814  0.00000000  0.00000000  0.02267176 -0.00000000
          3   H            X -0.00000000 -0.02927595  0.23101629 -0.00000000 -0.64326004
                           Y -0.00000000  0.23777094  0.04641325 -0.00000000 -0.25019888
                           Z  0.46974713  0.00000000  0.00000000  0.12677581 -0.00000000

         TRANS. SAYVETZ    X -0.00000000 -0.83563375  4.16074267 -0.00000000 -0.02228604
                           Y -0.00000000  4.15926402  0.83593088 -0.00000000  0.11091595
                           Z  1.03229856  0.00000000  0.00000000  4.11641335 -0.00000000
                       TOTAL  1.03229856  4.24237681  4.24388501  4.11641335  0.11313273

           ROT. SAYVETZ    X  0.74353714 -0.00000000 -0.00000000 -0.18361186 -0.00000000
                           Y -1.26256812  0.00000000  0.00000000  0.31924861  0.00000000
                           Z  0.00000000 -0.06777613  0.00000119  0.00000000  2.54154460
                       TOTAL  1.46523914  0.06777613  0.00000119  0.36828385  2.54154460

                                  6           7           8           9
               FREQUENCY:         8.88     1799.28     3812.34     3945.80  
                SYMMETRY:         A           A           A           A   
            REDUCED MASS:      1.01756     1.08983     1.03858     1.08500
            IR INTENSITY:      0.86226     1.89217     0.00115     0.21702

          1   O            X  0.00000000 -0.04089486 -0.02564877 -0.05626299
                           Y -0.00000000 -0.05786491 -0.03630837  0.03975514
                           Z -0.02526058  0.00000000 -0.00000000 -0.00000000
          2   H            X  0.00000000  0.01882370  0.69075509  0.67710255
                           Y  0.00000000  0.67521698 -0.05628041  0.01073177
                           Z -0.47603300  0.00000000 -0.00000000  0.00000000
          3   H            X -0.00000000  0.63020849 -0.28369066  0.21583219
                           Y -0.00000000  0.24314193  0.63252054 -0.64167502
                           Z  0.86919577 -0.00000000 -0.00000000  0.00000000

         TRANS. SAYVETZ    X -0.00000000  0.00000129 -0.00000014  0.00000052
                           Y  0.00000000  0.00000111  0.00000004 -0.00000057
                           Z -0.00780139  0.00000000 -0.00000000  0.00000000
                       TOTAL  0.00780139  0.00000170  0.00000015  0.00000077

           ROT. SAYVETZ    X  1.50357589 -0.00000000  0.00000000  0.00000000
                           Y  1.38590886 -0.00000000  0.00000000 -0.00000000
                           Z  0.00000000 -0.00001496 -0.00000000  0.00000153
                       TOTAL  2.04486768  0.00001496  0.00000000  0.00000153

         REFERENCE ON SAYVETZ CONDITIONS - A. SAYVETZ, J.CHEM.PHYS., 7, 383-389(1939).

         NOTE - THE MODES J,K ARE ORTHONORMALIZED ACCORDING TO
         SUM ON I   M(I) * (X(I,J)*X(I,K) + Y(I,J)*Y(I,K) + Z(I,J)*Z(I,K)) = DELTA(J,K)

             -------------------------------
             THERMOCHEMISTRY AT T=  298.15 K
             -------------------------------

         USING IDEAL GAS, RIGID ROTOR, HARMONIC NORMAL MODE APPROXIMATIONS.
         P=  1.01325E+05 PASCAL.
         ALL FREQUENCIES ARE SCALED BY   1.00000
         THE MOMENTS OF INERTIA ARE (IN AMU*BOHR**2)
              2.07948     4.38456     6.46404
         THE ROTATIONAL SYMMETRY NUMBER IS  1.0
         THE ROTATIONAL CONSTANTS ARE (IN GHZ)
            867.08597   411.23564   278.94127
         THE HARMONIC ZERO POINT ENERGY IS (SCALED BY   1.000)
                0.021773 HARTREE/MOLECULE     4778.712676 CM**-1/MOLECULE 
               13.663039 KCAL/MOL               57.166155 KJ/MOL

                       Q               LN Q
         ELEC.     1.00000E+00       0.000000
         TRANS.    3.00431E+06      14.915558
         ROT.      8.69029E+01       4.464791
         VIB.      1.00017E+00       0.000170
         TOT.      2.61127E+08      19.380518

                      E         H         G         CV        CP        S
                   KJ/MOL    KJ/MOL    KJ/MOL   J/MOL-K   J/MOL-K   J/MOL-K
         ELEC.      0.000     0.000     0.000     0.000     0.000     0.000
         TRANS.     3.718     6.197   -36.975    12.472    20.786   144.800
         ROT.       3.718     3.718   -11.068    12.472    12.472    49.594
         VIB.      57.170    57.170    57.166     0.106     0.106     0.014
         TOTAL     64.607    67.086     9.123    25.050    33.364   194.407
         VIB. THERMAL CORRECTION E(T)-E(0) = H(T)-H(0) =     3.649 J/MOL

                      E         H         G         CV        CP        S
                 KCAL/MOL  KCAL/MOL  KCAL/MOL CAL/MOL-K CAL/MOL-K CAL/MOL-K
         ELEC.      0.000     0.000     0.000     0.000     0.000     0.000
         TRANS.     0.889     1.481    -8.837     2.981     4.968    34.608
         ROT.       0.889     0.889    -2.645     2.981     2.981    11.853
         VIB.      13.664    13.664    13.663     0.025     0.025     0.003
         TOTAL     15.441    16.034     2.180     5.987     7.974    46.464
         VIB. THERMAL CORRECTION E(T)-E(0) = H(T)-H(0) =     0.872 CAL/MOL
         ......END OF NORMAL COORDINATE ANALYSIS......

Visualise the normal modes
--------------------------

Open the output file in wxMacMolPlt. List the normal modes with Subwindow/Frequencies.

If you click on any mode, the main window will update to show you the displacement vectors associated with it. You can animate the vibration with View/Animate Mode.
