# Generating a Database for "A 2-3 mm high-resolution molecular line survey towards the centre of the nearby spiral galaxy NGC 6946" https://arxiv.org/abs/2201.02209

This routine is used by the group lead by Frank Bigiel in Bonn. 
Several modules have been created by Adam Leroy and Erik Rosowlosky (written in idl). 
Jakob den Brok together with Ivana Beslic translated it to python;

__version__ = "Molecular-Fireworks-in-NGC6946"
for the paper: https://arxiv.org/abs/2201.02209
(We plan to make the data presented in this paper public via the PHANGS CADC repository in the future)

__author__  = "C. Eibensteiner"

__email__   = "eibensteiner@astro.uni-bonn.de"

__credits__ = ["J. den Brok", "A. Leroy ", "I. Beslic", "E. Rosowlosky",
               "F. Bigiel", "M.J. Jimenez-Donaire", "L. Neumann", "A. T. Barnes", "J. Puschnig"]
               
               

MODIFICATION HISTORY
* v1.0.1 16-22 October 2019: Conversion from IDL to Python
        Minor changes implemented (J. den Brok, I. Beslic )
* v1.1.1 26 October 2020: More stable version. Several bugs fixed.
        Additional scripts and functions (J. den Brok, I. Beslic, C.Eibensteiner, L. Neumann).
        Used by group lead by Frank Bigiel, Bonn
* version: Molecular-Fireworks-in-NGC6946 (for paper: https://arxiv.org/abs/2201.02209)


# Generating a database

This repository contains the python scripts that sets up 3 python dictionaries which have been used in this paper: https://arxiv.org/abs/2201.02209. 
The main file is the `create_database_NGC6946.py` -- that creates a dictornary which contains: 

*  The fits files that have been defined in the `List_Files` directory in the `band_list_ngc6946.csv` and the `cube_list_ngc6946.csv` files.

The two other `create_database.py` create dictonaries that are discussed together with EMPIRE dense gas data in the Section 6.3. They contain:

* M51 observations (from paper: https://ui.adsabs.harvard.edu/abs/2016A%26A...593A.118Q/abstract)
* NGC3627 observations (from paper: https://ui.adsabs.harvard.edu/abs/2021MNRAS.506..963B/abstract)

**(!) What each function does is described in the indivdual modules**


