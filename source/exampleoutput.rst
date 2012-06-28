Looking at GAMESS output
========================

When you run GAMESS, an output file (or "log file") is created. This is a text file that contains all of the results of the calculation.

Example output file
-------------------

The following output file (available as a 6-page PDF here_) is the result of a single point RHF/STO-3G calculation on a water molecule. A series of questions follows.

.. _here: _static/water_sym.out.pdf


::

         Distributed Data Interface kickoff program.
         Initiating 2 compute processes on 2 nodes to run the following command:
         C:\WinGAMESS/gamess.10.exe water_sym 

                  ******************************************************
                  *         GAMESS VERSION =  1 OCT 2010 (R1)          *
                  *             FROM IOWA STATE UNIVERSITY             *
                  * M.W.SCHMIDT, K.K.BALDRIDGE, J.A.BOATZ, S.T.ELBERT, *
                  *   M.S.GORDON, J.H.JENSEN, S.KOSEKI, N.MATSUNAGA,   *
                  *          K.A.NGUYEN, S.J.SU, T.L.WINDUS,           *
                  *       TOGETHER WITH M.DUPUIS, J.A.MONTGOMERY       *
                  *         J.COMPUT.CHEM.  14, 1347-1363(1993)        *
                  **************** 32 BIT LINUX VERSION ****************

          SINCE 1993, STUDENTS AND POSTDOCS WORKING AT IOWA STATE UNIVERSITY
          AND ALSO IN THEIR VARIOUS JOBS AFTER LEAVING ISU HAVE MADE IMPORTANT
          CONTRIBUTIONS TO THE CODE:
             IVANA ADAMOVIC, CHRISTINE AIKENS, YURI ALEXEEV, POOJA ARORA,
             ANDREY ASADCHEV, ROB BELL, PRADIPTA BANDYOPADHYAY, JONATHAN BENTZ,
             BRETT BODE, GALINA CHABAN, WEI CHEN, CHEOL HO CHOI, PAUL DAY, TIM DUDLEY,
             DMITRI FEDOROV, GRAHAM FLETCHER, MARK FREITAG, KURT GLAESEMANN, DAN KEMP,
             GRANT MERRILL, NORIYUKI MINEZAWA, JONATHAN MULLIN, TAKESHI NAGATA,
             SEAN NEDD, HEATHER NETZLOFF, BOSILJKA NJEGIC, RYAN OLSON, MIKE PAK,
             JIM SHOEMAKER, LYUDMILA SLIPCHENKO, SAROM SOK, JIE SONG,
             TETSUYA TAKETSUGU, SIMON WEBB, SOOHAENG YOO, FEDERICO ZAHARIEV

          ADDITIONAL CODE HAS BEEN PROVIDED BY COLLABORATORS IN OTHER GROUPS:
             IOWA STATE UNIVERSITY:
                  JOE IVANIC, LAIMUTIS BYTAUTAS, KLAUS RUEDENBERG
             UNIVERSITY OF TOKYO: KIMIHIKO HIRAO, TAKAHITO NAKAJIMA,
                  TAKAO TSUNEDA, MUNEAKI KAMIYA, SUSUMU YANAGISAWA,
                  KIYOSHI YAGI, MAHITO CHIBA, SEIKEN TOKURA, NAOAKI KAWAKAMI
             UNIVERSITY OF AARHUS: FRANK JENSEN
             UNIVERSITY OF IOWA: VISVALDAS KAIRYS, HUI LI
             NATIONAL INST. OF STANDARDS AND TECHNOLOGY: WALT STEVENS, DAVID GARMER
             UNIVERSITY OF PISA: BENEDETTA MENNUCCI, JACOPO TOMASI
             UNIVERSITY OF MEMPHIS: HENRY KURTZ, PRAKASHAN KORAMBATH
             UNIVERSITY OF ALBERTA: TOBY ZENG, MARIUSZ KLOBUKOWSKI
             UNIVERSITY OF NEW ENGLAND: MARK SPACKMAN
             MIE UNIVERSITY: HIROAKI UMEDA
             MICHIGAN STATE UNIVERSITY:
                  KAROL KOWALSKI, MARTA WLOCH, JEFFREY GOUR, JESSE LUTZ, PIOTR PIECUCH
             UNIVERSITY OF SILESIA: MONIKA MUSIAL, STANISLAW KUCHARSKI
             FACULTES UNIVERSITAIRES NOTRE-DAME DE LA PAIX:
                  OLIVIER QUINET, BENOIT CHAMPAGNE
             UNIVERSITY OF CALIFORNIA - SANTA BARBARA: BERNARD KIRTMAN
             INSTITUTE FOR MOLECULAR SCIENCE:
                  KAZUYA ISHIMURA, MICHIO KATOUDA, AND SHIGERU NAGASE
             UNIVERSITY OF NOTRE DAME: DAN CHIPMAN
             KYUSHU UNIVERSITY:
                  HARUYUKI NAKANO,
                  FENG LONG GU, JACEK KORCHOWIEC, MARCIN MAKOWSKI, AND YURIKO AOKI,
                  HIROTOSHI MORI AND EISAKU MIYOSHI
             PENNSYLVANIA STATE UNIVERSITY:
                  TZVETELIN IORDANOV, CHET SWALINA, JONATHAN SKONE,
                  SHARON HAMMES-SCHIFFER
             WASEDA UNIVERSITY:
                  MASATO KOBAYASHI, TOMOKO AKAMA, HIROMI NAKAI
             UNIVERSITY OF NEBRASKA:
                  PEIFENG SU, DEJUN SI, YALI WANG, HUI LI
             UNIVERSITY OF ZURICH:
                  ROBERTO PEVERATI, KIM BALDRIDGE
             N. COPERNICUS UNIVERSITY AND JACKSON STATE UNIVERSITY:
                  MARIA BARYSZ


         PARALLEL VERSION RUNNING ON     2 PROCESSORS IN     2 NODES.

         EXECUTION OF GAMESS BEGUN Mon Apr 11 13:58:57 2011

                    ECHO OF THE FIRST FEW INPUT CARDS -
         INPUT CARD>!   File created by MacMolPlt 7.4                                               
         INPUT CARD> $CONTRL SCFTYP=RHF RUNTYP=ENERGY MAXIT=30 MULT=1 $END                          
         INPUT CARD> $SYSTEM TIMLIM=525600 MEMORY=1000000 $END                                      
         INPUT CARD> $BASIS GBASIS=STO NGAUSS=3 $END                                                
         INPUT CARD> $SCF DIRSCF=.TRUE. $END                                                        
         INPUT CARD> $DATA                                                                          
         INPUT CARD>Title                                                                           
         INPUT CARD>CNV 2                                                                           
         INPUT CARD>                                                                                
         INPUT CARD>O     8.0     0.00000     0.00000    -0.06673                                   
         INPUT CARD>H     1.0     0.76334     0.00000     0.52965                                   
         INPUT CARD> $END                                                                           
            1000000 WORDS OF MEMORY AVAILABLE

             BASIS OPTIONS
             -------------
             GBASIS=STO          IGAUSS=       3      POLAR=NONE    
             NDFUNC=       0     NFFUNC=       0     DIFFSP=       F
             NPFUNC=       0      DIFFS=       F     BASNAM=        


             RUN TITLE
             ---------
         Title                                                                           

         THE POINT GROUP OF THE MOLECULE IS CNV     
         THE ORDER OF THE PRINCIPAL AXIS IS     2

         ATOM      ATOMIC                      COORDINATES (BOHR)
                   CHARGE         X                   Y                   Z
         O           8.0     0.0000000000        0.0000000000       -0.1261014152
         H           1.0    -1.4425034355        0.0000000000        1.0008933694
         H           1.0     1.4425034355        0.0000000000        1.0008933694

                  INTERNUCLEAR DISTANCES (ANGS.)
                  ------------------------------

                        1 O          2 H          3 H     

           1 O       0.0000000    0.9686883 *  0.9686883 *
           2 H       0.9686883 *  0.0000000    1.5266800 *
           3 H       0.9686883 *  1.5266800 *  0.0000000  

          * ... LESS THAN  3.000


             ATOMIC BASIS SET
             ----------------
         THE CONTRACTED PRIMITIVE FUNCTIONS HAVE BEEN UNNORMALIZED
         THE CONTRACTED BASIS FUNCTIONS ARE NOW NORMALIZED TO UNITY

          SHELL TYPE  PRIMITIVE        EXPONENT          CONTRACTION COEFFICIENT(S)

         O         

              1   S       1           130.7093214    0.154328967295
              1   S       2            23.8088661    0.535328142282
              1   S       3             6.4436083    0.444634542185

              2   L       4             5.0331513   -0.099967229187    0.155916274999
              2   L       5             1.1695961    0.399512826089    0.607683718598
              2   L       6             0.3803890    0.700115468880    0.391957393099

         H         

              4   S       7             3.4252509    0.154328967295
              4   S       8             0.6239137    0.535328142282
              4   S       9             0.1688554    0.444634542185

         TOTAL NUMBER OF BASIS SET SHELLS             =    4
         NUMBER OF CARTESIAN GAUSSIAN BASIS FUNCTIONS =    7
         NUMBER OF ELECTRONS                          =   10
         CHARGE OF MOLECULE                           =    0
         SPIN MULTIPLICITY                            =    1
         NUMBER OF OCCUPIED ORBITALS (ALPHA)          =    5
         NUMBER OF OCCUPIED ORBITALS (BETA )          =    5
         TOTAL NUMBER OF ATOMS                        =    3
         THE NUCLEAR REPULSION ENERGY IS        9.0871358664

             $CONTRL OPTIONS
             ---------------
         SCFTYP=RHF          RUNTYP=ENERGY       EXETYP=RUN     
         MPLEVL=       0     CITYP =NONE         CCTYP =NONE         VBTYP =NONE    
         DFTTYP=NONE         TDDFT =NONE    
         MULT  =       1     ICHARG=       0     NZVAR =       0     COORD =UNIQUE  
         PP    =NONE         RELWFN=NONE         LOCAL =NONE         NUMGRD=       F
         ISPHER=      -1     NOSYM =       0     MAXIT =      30     UNITS =ANGS    
         PLTORB=       F     MOLPLT=       F     AIMPAC=       F     FRIEND=        
         NPRINT=       7     IREST =       0     GEOM  =INPUT   
         NORMF =       0     NORMP =       0     ITOL  =      20     ICUT  =       9
         INTTYP=BEST         GRDTYP=BEST         QMTTOL= 1.0E-06

             $SYSTEM OPTIONS
             ---------------
          REPLICATED MEMORY=     1000000 WORDS (ON EVERY NODE).
         DISTRIBUTED MEMDDI=           0 MILLION WORDS IN AGGREGATE,
         MEMDDI DISTRIBUTED OVER   2 PROCESSORS IS           0 WORDS/PROCESSOR.
         TOTAL MEMORY REQUESTED ON EACH PROCESSOR=     1000000 WORDS.
         TIMLIM=      525600.00 MINUTES, OR     365.0 DAYS.
         PARALL= T  BALTYP=  DLB     KDIAG=    0  COREFL= F
         MXSEQ2=     300 MXSEQ3=     150

                  ----------------
                  PROPERTIES INPUT
                  ----------------

             MOMENTS            FIELD           POTENTIAL          DENSITY
         IEMOM =       1   IEFLD =       0   IEPOT =       0   IEDEN =       0
         WHERE =COMASS     WHERE =NUCLEI     WHERE =NUCLEI     WHERE =NUCLEI  
         OUTPUT=BOTH       OUTPUT=BOTH       OUTPUT=BOTH       OUTPUT=BOTH    
         IEMINT=       0   IEFINT=       0                     IEDINT=       0
                                                               MORB  =       0
                  EXTRAPOLATION IN EFFECT
         ORBITAL PRINTING OPTION: NPREO=     1     7     2     1

             -------------------------------
             INTEGRAL TRANSFORMATION OPTIONS
             -------------------------------
             NWORD  =            0
             CUTOFF = 1.0E-09     MPTRAN =       0
             DIRTRF =       T     AOINTS =DUP     

                  ----------------------
                  INTEGRAL INPUT OPTIONS
                  ----------------------
         NOPK  =       1 NORDER=       0 SCHWRZ=       T

             ------------------------------------------
             THE POINT GROUP IS CNV, NAXIS= 2, ORDER= 4
             ------------------------------------------

             DIMENSIONS OF THE SYMMETRY SUBSPACES ARE
         A1  =    4     A2  =    0     B1  =    2     B2  =    1

         ..... DONE SETTING UP THE RUN .....
         CPU     0: STEP CPU TIME=     0.02 TOTAL CPU TIME=        0.0 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.0 SECONDS, CPU UTILIZATION IS  93.75%

                  ********************
                  1 ELECTRON INTEGRALS
                  ********************
         ...... END OF ONE-ELECTRON INTEGRALS ......
         CPU     0: STEP CPU TIME=     0.00 TOTAL CPU TIME=        0.0 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.0 SECONDS, CPU UTILIZATION IS  93.75%

                  -------------
                  GUESS OPTIONS
                  -------------
                  GUESS =HUCKEL            NORB  =       0          NORDER=       0
                  MIX   =       F          PRTMO =       F          PUNMO =       F
                  TOLZ  = 1.0E-08          TOLE  = 1.0E-05
                  SYMDEN=       F          PURIFY=       F

         INITIAL GUESS ORBITALS GENERATED BY HUCKEL   ROUTINE.
         HUCKEL GUESS REQUIRES      2569 WORDS.

         SYMMETRIES FOR INITIAL GUESS ORBITALS FOLLOW.   BOTH SET(S).
             5 ORBITALS ARE OCCUPIED (    1 CORE ORBITALS).
             2=A1       3=B1       4=A1       5=B2       6=B1       7=A1  
         ...... END OF INITIAL ORBITAL SELECTION ......
         CPU     0: STEP CPU TIME=     0.00 TOTAL CPU TIME=        0.0 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.0 SECONDS, CPU UTILIZATION IS  93.75%

                            ----------------------
                            AO INTEGRAL TECHNOLOGY
                            ----------------------
             S,P,L SHELL ROTATED AXIS INTEGRALS, REPROGRAMMED BY
                KAZUYA ISHIMURA (IMS) AND JOSE SIERRA (SYNSTAR).
             S,P,D,L SHELL ROTATED AXIS INTEGRALS PROGRAMMED BY
                KAZUYA ISHIMURA (INSTITUTE FOR MOLECULAR SCIENCE).
             S,P,D,F,G SHELL TO TOTAL QUARTET ANGULAR MOMENTUM SUM 5,
                ERIC PROGRAM BY GRAHAM FLETCHER (ELORET AND NASA ADVANCED
                SUPERCOMPUTING DIVISION, AMES RESEARCH CENTER).
             S,P,D,F,G,L SHELL GENERAL RYS QUADRATURE PROGRAMMED BY
                MICHEL DUPUIS (PACIFIC NORTHWEST NATIONAL LABORATORY).

                  --------------------
                  2 ELECTRON INTEGRALS
                  --------------------

         DIRECT SCF METHOD SKIPS INTEGRAL STORAGE ON DISK.
         DIRECT TRANSFORMATION SKIPS AO INTEGRAL STORAGE ON DISK.
          ...... END OF TWO-ELECTRON INTEGRALS .....
         CPU     0: STEP CPU TIME=     0.05 TOTAL CPU TIME=        0.1 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.1 SECONDS, CPU UTILIZATION IS  79.49%

                  --------------------------
                         RHF SCF CALCULATION
                  --------------------------

             NUCLEAR ENERGY =         9.0871358664
             MAXIT =   30     NPUNCH=    2
             EXTRAP=T  DAMP=F  SHIFT=F  RSTRCT=F  DIIS=F  DEM=F  SOSCF=F
             DENSITY MATRIX CONV=  2.00E-05
             MEMORY REQUIRED FOR RHF ITERS=     44817 WORDS.

         DIRECT SCF CALCULATION, SCHWRZ=T   FDIFF=T,  DIRTHR=  0.00E+00 NITDIR=10
         SCHWARZ INEQUALITY OVERHEAD:        28 INTEGRALS, T=        0.00

                                                                                           NONZERO     BLOCKS
         ITER EX DEM     TOTAL ENERGY        E CHANGE  DENSITY CHANGE    DIIS ERROR      INTEGRALS    SKIPPED
           1  0  0      -74.7974092796   -74.7974092796   0.596869468   0.000000000            141          0
           2  1  0      -74.9507257506    -0.1533164709   0.181657794   0.000000000            141          0
           3  2  0      -74.9629281338    -0.0122023833   0.059598419   0.000000000            141          0
           4  3  0      -74.9642035242    -0.0012753904   0.020216252   0.000000000            141          0
           5  4  0      -74.9643795359    -0.0001760117   0.007366384   0.000000000            141          0
           6  0  0      -74.9644088533    -0.0000293174   0.004742101   0.000000000            141          0
           7  1  0      -74.9644154231    -0.0000065699   0.000070104   0.000000000            141          0
           8  2  0      -74.9644154252    -0.0000000021   0.000025327   0.000000000            141          0
           9  3  0      -74.9644154256    -0.0000000003   0.000009752   0.000000000            141          0

                  -----------------
                  DENSITY CONVERGED
                  -----------------
             TIME TO FORM FOCK OPERATORS=       0.0 SECONDS (       0.0 SEC/ITER)
             FOCK TIME ON FIRST ITERATION=       0.0, LAST ITERATION=       0.0
             TIME TO SOLVE SCF EQUATIONS=       0.0 SECONDS (       0.0 SEC/ITER)

         FINAL RHF ENERGY IS      -74.9644154256 AFTER   9 ITERATIONS

                  ------------
                  EIGENVECTORS
                  ------------

                              1          2          3          4          5
                          -20.2438    -1.2632    -0.6111    -0.4529    -0.3909
                             A1         A1         B1         A1         B2  
            1  O  1  S    0.994158  -0.233200  -0.000000   0.102889   0.000000
            2  O  1  S    0.026315   0.837618  -0.000000  -0.534598   0.000000
            3  O  1  X   -0.000000   0.000000   0.606792  -0.000000   0.000000
            4  O  1  Y   -0.000000   0.000000  -0.000000  -0.000000   1.000000
            5  O  1  Z    0.004251   0.126155  -0.000000   0.772609   0.000000
            6  H  2  S   -0.005841   0.157816  -0.446042   0.282964   0.000000
            7  H  3  S   -0.005841   0.157816   0.446042   0.282964   0.000000

                              6          7
                            0.5952     0.7274
                             A1         B1  
            1  O  1  S   -0.130529   0.000000
            2  O  1  S    0.863693   0.000000
            3  O  1  X    0.000000   0.982566
            4  O  1  Y    0.000000   0.000000
            5  O  1  Z    0.744429   0.000000
            6  H  2  S   -0.788315   0.828700
            7  H  3  S   -0.788315  -0.828700
         ...... END OF RHF CALCULATION ......
         CPU     0: STEP CPU TIME=     0.00 TOTAL CPU TIME=        0.1 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.1 SECONDS, CPU UTILIZATION IS  79.49%

             ----------------------------------------------------------------
             PROPERTY VALUES FOR THE RHF   SELF-CONSISTENT FIELD WAVEFUNCTION
             ----------------------------------------------------------------

                  -----------------
                  ENERGY COMPONENTS
                  -----------------

                 WAVEFUNCTION NORMALIZATION =       1.0000000000

                        ONE ELECTRON ENERGY =    -122.1793235802
                        TWO ELECTRON ENERGY =      38.1277722882
                   NUCLEAR REPULSION ENERGY =       9.0871358664
                                              ------------------
                               TOTAL ENERGY =     -74.9644154256

         ELECTRON-ELECTRON POTENTIAL ENERGY =      38.1277722882
          NUCLEUS-ELECTRON POTENTIAL ENERGY =    -196.7417484352
           NUCLEUS-NUCLEUS POTENTIAL ENERGY =       9.0871358664
                                              ------------------
                     TOTAL POTENTIAL ENERGY =    -149.5268402806
                       TOTAL KINETIC ENERGY =      74.5624248550
                         VIRIAL RATIO (V/T) =       2.0053913291

          ...... PI ENERGY ANALYSIS ......

         ENERGY ANALYSIS:
                    FOCK ENERGY=    -45.9237766278
                  BARE H ENERGY=   -122.1793235802
             ELECTRONIC ENERGY =    -84.0515501040
                 KINETIC ENERGY=     74.5624248550
                  N-N REPULSION=      9.0871358664
                   TOTAL ENERGY=    -74.9644142376
                SIGMA PART(1+2)=    -76.2127294486
                       (K,V1,2)=     69.5049624030   -176.7884643168     31.0707724652
                   PI PART(1+2)=     -7.8388206554
                       (K,V1,2)=      5.0574624520    -19.9532841185      7.0570010110
          SIGMA SKELETON, ERROR=    -67.1255935822      0.0000000000
                     MIXED PART= 0.00000E+00 0.00000E+00 0.00000E+00 0.00000E+00
         ...... END OF PI ENERGY ANALYSIS ......

                  ---------------------------------------
                  MULLIKEN AND LOWDIN POPULATION ANALYSES
                  ---------------------------------------

             ATOMIC MULLIKEN POPULATION IN EACH MOLECULAR ORBITAL

                              1          2          3          4          5

                          2.000000   2.000000   2.000000   2.000000   2.000000

            1             2.001361   1.617307   1.068623   1.667555   2.000000
            2            -0.000680   0.191347   0.465688   0.166222   0.000000
            3            -0.000680   0.191347   0.465688   0.166222   0.000000

                       ----- POPULATIONS IN EACH AO -----
                                     MULLIKEN      LOWDIN
                      1  O  1  S      1.99768     1.99607
                      2  O  1  S      1.83410     1.68593
                      3  O  1  X      1.06862     1.09728
                      4  O  1  Y      2.00000     2.00000
                      5  O  1  Z      1.45445     1.46728
                      6  H  2  S      0.82258     0.87672
                      7  H  3  S      0.82258     0.87672

                  ----- MULLIKEN ATOMIC OVERLAP POPULATIONS -----
                  (OFF-DIAGONAL ELEMENTS NEED TO BE MULTIPLIED BY 2)

                     1           2           3

            1    7.8326767
            2    0.2610849   0.6079246
            3    0.2610849  -0.0464327   0.6079246

                  TOTAL MULLIKEN AND LOWDIN ATOMIC POPULATIONS
               ATOM         MULL.POP.    CHARGE          LOW.POP.     CHARGE
            1 O             8.354846   -0.354846         8.246557   -0.246557
            2 H             0.822577    0.177423         0.876722    0.123278
            3 H             0.822577    0.177423         0.876722    0.123278

                  -------------------------------
                  BOND ORDER AND VALENCE ANALYSIS     BOND ORDER THRESHOLD=0.050
                  -------------------------------

                           BOND                       BOND                       BOND
          ATOM PAIR DIST  ORDER      ATOM PAIR DIST  ORDER      ATOM PAIR DIST  ORDER
            1   2  0.969  0.957        1   3  0.969  0.957

                               TOTAL       BONDED        FREE
              ATOM            VALENCE     VALENCE     VALENCE
            1 O                 1.913       1.913       0.000
            2 H                 0.969       0.969       0.000
            3 H                 0.969       0.969       0.000

                  ---------------------
                  ELECTROSTATIC MOMENTS
                  ---------------------

         POINT   1           X           Y           Z (BOHR)    CHARGE
                         0.000000    0.000000    0.000026        0.00 (A.U.)
                 DX          DY          DZ         /D/  (DEBYE)
             0.000000    0.000000    1.713972    1.713972
         ...... END OF PROPERTY EVALUATION ......
         CPU     0: STEP CPU TIME=     0.02 TOTAL CPU TIME=        0.1 (    0.0 MIN)
         TOTAL WALL CLOCK TIME=        0.1 SECONDS, CPU UTILIZATION IS  81.91%
              580000  WORDS OF DYNAMIC MEMORY USED
         EXECUTION OF GAMESS TERMINATED NORMALLY Mon Apr 11 13:58:57 2011
         DDI: 263224 bytes (0.3 MB / 0 MWords) used by master data server.

         ----------------------------------------
         CPU timing information for all processes
         ========================================
         0: 0.171 + 0.62 = 0.233
         1: 0.140 + 0.00 = 0.140
         2: 0.00 + 0.15 = 0.15
         3: 0.00 + 0.31 = 0.31
         ----------------------------------------
         ddikick.x: exited gracefully.
        ----- accounting info -----

Questions
---------

.. rubric:: INPUT CARD

The ``INPUT CARD`` section at the start shows the first few lines of the input file. Here it shows the entire input. 

1. Can you figure out from the input file that this is a RHF/STO-3G calculation?

2. The input file appears to only specify the coordinates for two atoms, an oxygen and a hydrogen. How does GAMESS know that there is a second hydrogen? (Hint: see the section after ``RUN TITLE``.)

.. rubric:: INTERNUCLEAR DISTANCES

1. In the ``INTERNUCELAR DISTANCES`` section, what is the point of the asterisks after some of the distance values?

.. rubric:: ATOMIC BASIS SET

1. How many basis functions are there? Can you work out what basis functions they are? (Hint: see the ``EIGENVECTORS`` section.)

2. How many occupied orbitals are there?

3. Neutral water has 10 electrons, and a spin multiplicity (number of unpaired electrons + 1) of 1. If a molecule had 11 electrons, what values for multiplicity would be possible?

.. rubric:: $SYSTEM OPTIONS

The amount of memory available to GAMESS can be set using the ``MWORDS`` command (megawords) in the ``$SYSTEM`` section. The value of MWORDS defaults to 1 (i.e. 1000000 words).

1. If 1 `word` is 8 bytes, how many MB of memory are available to GAMESS by default? Given that modern computers have 2GB or more of RAM, is it safe to increase this value if GAMESS complains about running out of memory?

.. rubric:: RHF SCF CALCULATIONS

Much of the computation time in a typical calculation is spent in the SCF section. This is an iterative procedure that keeps repeating until the difference between the density matrix on successive iterations is less than 0.00002.

1. How many iterations did it take for SCF convergence? What was the final energy?

2. Would you say that the SCF converges nicely in this case? What would you expect to see if there was a problem converging the SCF?

3. Could you make a guess about the meaning of ``MAXIT =   30``? Can you think of any circumstance where it might be useful to increase this value?

.. rubric:: EIGENVECTORS

The eigenvectors of a QM calculation are the molecular orbitals. Each molecular orbital is described in terms of the basis functions.

1. How many molecular orbitals are there?

2. Which eigenvector represents the HOMO? What is its energy? Where is the HOMO located?

3. Which eigenvector represents the LUMO? What is its energy?

.. rubric:: MULLIKEN AND LOWDIN POPULATION ANALYSES

1. What are the Mulliken charges on each atom? Do they make sense?
