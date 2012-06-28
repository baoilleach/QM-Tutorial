Install required software
=========================

The following instructions describe how to obtain and install GAMESS, Avogadro and wxMacMolPlt on Windows (as of April 2011). 

.. rubric:: Install GAMESS

1. Follow the "How to get GAMESS" link from the `GAMESS website`_. When you finally get to the download page, enter your email address and tick the box for "GAMESS version October 1, 2010 R1 for Microsoft Windows", and click :guilabel:`Submit Request`.

2. After a couple of minutes, you will receive an email containing a link to the WinGAMESS download along with a password. Click on the link and enter the password to download the installer. Run the installer and choose all of the defaults. In particular, you should make sure to install to :file:`C:/WinGAMESS`.

3. You need to correct an error in :file:`C:/WinGAMESS/WG_DDE.bat`. Open the :file:`C:/WinGAMESS` folder, right-click on :file:`C:/WinGAMESS/WG_DDE.bat` and choose :guilabel:`Edit`. Change line 40 of the file to read as follows::

    set WinGamess_Version=10

  Naturally, if you are using a different version of GAMESS, you should set this value appropriately.

4. To test your GAMESS installation, save this GAMESS input file `ethane.inp <_static/ethane.inp>`_ on your Desktop, open the folder :file:`C:/WinGAMESS`, and drag-and-drop :file:`ethane.inp` onto :file:`WG_DDE.bat`. The first time you do this, you may have to say Yes twice to allow it through the Windows firewall (this requires Administrator rights). If GAMESS is working properly, it will create a file :file:`ethane.out` on your Desktop.

.. rubric:: Install Avogadro

Download **Avogadro** 1.0.1 from http://avogadro.openmolecules.net, using the :guilabel:`Get Avogadro` link. Run the installer.

.. rubric:: Install wxMacMolPlt

**wxMacmolPlot** 7.4.2 is available from http://www.scl.ameslab.gov/MacMolPlt/. The download link is towards the bottom of the page. Run the installer.

.. _GAMESS website: http://www.msg.chem.iastate.edu/GAMESS/GAMESS.html
