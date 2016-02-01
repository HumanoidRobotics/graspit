# COMSE 6731 HUMANOID ROBOTS, SPRING 2016
# Columbia University

## Installation
These packages have already been installed on the CLIC lab machines, if you are trying to set this up on your own machine, you will need to install the following for Ubuntu 14.04, it may be different for other OS's:

```bash
$ sudo apt-get install libqt4-opengl-dev
$ sudo apt-get install libqt4-dev
$ sudo apt-get install libqt4-sql-psql
$ sudo apt-get install libcoin80-dev 
$ sudo apt-get install libsoqt4-dev 
$ sudo apt-get install libblas-dev 
$ sudo apt-get install liblapack-dev 
$ sudo apt-get install libqhull-dev
```

Getting Started:
```bash
$ git clone https://github.com/HumanoidRobotics/graspit
$ cd graspit
$ qmake-qt4 graspit.pro
$ make -j4
$ export GRASPIT=$PWD
$ ./bin/graspit
```

Running the EigenGrasp Planner:

1. Start GraspIt!
```bash
$ ./bin/graspit
```
2. File->Open->PlannerMug.xml
3. Grasp->EigenGrasp Planner...
4. Set Energy Formulation to Contacts and Quality
5. Press Init
6. Press >


User Manual available at:
http://www.cs.columbia.edu/~cmatei/graspit/html-manual/graspit-manual.html

This is a fork from: https://github.com/graspit-simulator/graspit

Original README:


                                 GraspIt!
                              Version 2.2.0 

Introduction 
------------
Please see the User Manual in doc/ for an introduction to GraspIt!, a list of
features, installation instructions, getting started examples, etc.

Disclaimer
----------
This is code that has been, and is currently being used, for research. There 
are still many unfinished pieces and plenty of ways to crash the system.  It's
by no means bullet proof. Please see the Introduction in the User Manual for 
more details.

Distribution Contents
---------------------

graspit.pro
graspit-core.pro
graspit-lib-LINUX.pro
graspit-lib-WINDOWS.pro
	      -  These are the main project files for GraspIt! that you can 
		 use to create your project that you can compile. Please see
		 the User Manual for installation instructions.

doc/          -  Documentation.  Contains both the User Manual and code 
		 Reference Manual. The User Manual contains installation 
		 instructions, pointers for getting started, examples, and 
		 trouble shooting and contact information.

images/       -  A place to put images saved from GraspIt!

include/      -  Header files for the main GraspIt! source code

LICENSE.txt   -  A copy of the license you accepted when you downloaded this.

models/       -  The geometry and configuration files for all the robots and
		objects.

plugins/      -  Examples for creating plugins that can be loaded into GraspIt! 
                 at run time, and can use GraspIt! without being statically linked
		 into GraspIt's main executable.

ply/          - Code for loading .ply files; see header files for authorship 
                information and detail.

qhull/	  - A popular package for computing n-dimensional convex hulls.
		This is used both for the contact system and to create grasp
	      wrench spaces.

README.txt    -  This file.

src/          -  The source code for GraspIt!.

src/DBase     - source code for the interface between GraspIt and the Columbia 
		Grasp Database

tinyxml/	  - a library for processing XML documents. See the header files 
		therein for license and author information for this package.

ui/	        -  The dialog windows and interfaces for GraspIt!.

worlds/       -  A place to save GraspIt! worlds.  Also includes a few
		examples.

Troubleshooting
---------------
Please check the user manual for troubleshooting and contact information!
