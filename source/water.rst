Molecular orbitals of water
===========================

Let's visualise the molecular orbitals of water at the HF/3-21G level of theory.

Create an initial 3D structure
------------------------------

Using Avogadro, we can create an initial structure of the water molecule. Simply choose the Draw Tool (|builder|), change the Element to Oxygen, tick the box for :guilabel:`Adjust Hydrogens`, and click anywhere in the View Window.

This will draw a single oxygen atom, and hydrogens will be added automatically to satisfy the oxygen atom's valency, giving H2O.

Now optimise the structure using the MMFF94 forcefield (Extensions/Optimize Geometry).

Generate the GAMESS input file
------------------------------

Under Extensions/GAMESS/Input Generator, choose ``Equilibrium Geometry`` to find the optimized geometry. Choose ``RHF`` for the method and ``3-21G`` for the basis set.

The other options should be left at their default of ``Gas`` phase calculation, ``Singlet`` multiplicity, and ``Neutral`` charge.

Click on :guilabel:`Generate...` to save the GAMESS input file to an appropriate location.

Run GAMESS
----------

Open a Windows folder showing the location of the GAMESS input file. Open another Windows folder showing the location where GAMESS was installed (typically :file:`C:/WinGAMESS`).

Now drag-and-drop the GAMESS input file on top of :file:`C:/WinGAMESS/WG_DDE.BAT`.

This will start the calculation, and the output will be written to a file with the same name and location as the input file, but with the extension :file:`.out`.

Investigate the geometry optimisation
-------------------------------------

Start wxMacMolPlt, and File/Open the output file from the GAMESS run.

The geometry optimisation probably involved several steps. You can use the slider at the bottom right of the wxMacMolPlot window to investigate the steps.

If you click on Subwindow/Energy Plot you can see a plot of the energy values and root-mean-squared change in coordinates for the steps.

Look at the electrostatic potential
-----------------------------------

The molecular electrostatic potential (MEP) is a measure of the force (attractive or repulsive) felt by a point charge at a certain point in space due to the electronic distribution in a molecule. We can colour the molecular surface using the MEP to give some idea of where nucleophiles or electrophiles might attack.

Here we will use an isosurface of the electron density to represent the molecular surface.

Click on Subwindow/Surfaces/"3D Total Electron Density". Click Update to generate a wireframe wire of an isosurface of the electron density.

.. note:: What the effect of increasing or decreasing the number of grid points, the grid size, or the contour value?

  It is worth remembering that the larger the contour value, the smaller the volume contained by the isosurface.

Set the number of grid points to 25, the counter value to 0.04, the Surface Display to Solid, tick the Smooth box and click Update.

To colour the surface using the MEP, tick "Colorize using the surface MEP value" and also "Invert color map". You may want to increase the Transparency to 20%, then click Update.

When finished admiring your work, click :guilabel:`Delete` to remove the surface.

Visualise the orbitals
----------------------

Now click Add.../"3D Orbital" to bring up the orbital visualiser settings.

Draw the HOMO using a smooth solid surface. Save a copy of the view using File/Export. Choose "Portable Network Graphics (\*.png)", the filename :file:`water_homo.png` and click :guilabel:`Save`. In the Export Options, choose "300dpi (Print)".

Do the same for the LUMO. How do they compare?

.. |builder| image:: _static/builder.png

