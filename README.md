# LieAlg

Maple package for computations in infinite-dimensional Lie algebras, representations and vertex algebras

(C) 1999-2019 - Yuly Billig (billig@math.carleton.ca) and Matyas Mazzag (matyas.mazzag@gmail.com)

Distributed under Open Source GNU AGPLv3 License
 
 
This repository contains the following files:

LieAlg_overview.mws - Maple worksheet with an overview of features of this package and examples

LieAlg_overview.pdf - same in PDF format

LieAlg.m - Maple executable with the open part of the package (contains functions available to the user)

LieAlg.m - Maple executable with the hidden part of the package (contains internal functions)

LieAlg_source.mws - complete open source for the code of the whole package

LieAlg.help - help database for the functions in the package

LieAlg.hdb - help database for the older versions of Maple
 
 
Installation Instructions:

Create a directory LIEALG

Download all files from this repository in directory LIEALG

To install help database, copy file LieAlg.help into MAPLE's lib directory

To find out precise path to lib, start a MAPLE worksheet and type libname;

A path to lib will appear in the output

If you use an older version of Maple (e.g. Maple 16), place file LieAlg.hdb in lib instead of LieAlg.help (but not both!)

To check that help works, close and open MAPLE and type ?unienv in a MAPLE worksheet. 

A help page for unienv function should appear. Help database needs to be installed only once.
 
 
Remaining steps should be performed each time you start a new worksheet where you plan to use LieAlg

Look up a full path for the LIEALG directory

Place a path to LIEALG as the first entry in libname

On Windows this will look like this (adjust the path!):

libname := "C:\\\\Users\\\\Yuly\\\\Documents\\\\MAPLE\\\\LIEALG", libname;

On Linux, something like that:

libname := "/home/yuly/MAPLE/LIEALG", libname;

Load files LieAlg.m and LieAlg_Hidden.m by typing (adjust the path!):

read "/home/yuly/MAPLE/LIEALG/LieAlg.m"; 

read "/home/yuly/MAPLE/LIEALG/LieAlg_Hidden.m";

Activate the package:

with(LieAlg);
 
 
It is recommended to start with the worksheet LieAlg_overview.mws to familiarize yourself with the package

That worksheet also has the above information/example with the activation of LieAlg
 
 
If for some reason you need to recreate the files LieAlg.m and LieAlg_Hidden.m, 

load LieAlg_source.mws into MAPLE and choose from the menu: Edit -> Execute -> Worksheet 
 
 
Please send bug reports to: billig@math.carleton.ca
 
