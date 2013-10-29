#Date: 10-28-2013
#Author: Michael Brothers
#Title: Newton Raphson Example Serial Implementation 

#Description: 

Contained in NewtonRaphsonExamples-master.tar.bz2 is a header-only interface
for solving nonlinear systems which works by using parts of the Trilinos agile
components library to provide data structures and to perform linear algebra
functions. 

Accompanying the interface are two example programs, NRExamples and
NRComparison, which are further derscribed within the archive. Their primary
purpose is to give users an idea of how to write their own serial Newton's
method solvers which use Automatic Differentiation or implement the Complex
Step method.

They are not appropriate for reasearch use. For instance a more flexible input
system should be developed and some multiprocessing support/ domain decomposition
needs to be implemented for any large-scale or serious use.

#Disclaimer: 

"this software" is defined as any information contained within the GITHUB
repository which was arranged by the instant authors for distribution which
pertains to the Peridigm Complex Step Jacobian research project.  Users accept
by using this software that it is for evaluation, educational and research
purposes only and is not intended for sale, transfer, or incorporation into
derived products intended for sale, especially to persons originating from
countries foreign to the United Stated of America, nor this software offered or
intended as a means to assess information pertaining to the safety, wellbeing
or integrity of persons or property. This software is distributed as is, free
of charge, under the conditions that this disclaimer be attached to any
derivative works and that if modified for the purpose of producing derivative
works the original and intact source code be distributed with the derivative
work and is accompanied by this disclaimer, to be applied to all subsequent
derivative works.

#Directions: 

Use the unix programs tar and bzip2 to extract the archive.

Given that your Trilinos libraries are located where allcompile.sh expects,
just run that script in a terminal to compile the examples.

NRExamples solves the problem of an intersection of ifinite paraboloids,
hardcoded into the program. The user can select solver paramters as prompted
in the terminal. Run the program with no argments and a message to std out 
will provide further instructions.

NRComparison solves a validation problem using information from another
research paper identified in the README with in the archive containing the
head-only interface. It sourcecode demonstrates how to drive the header-only
interface to solve problems which are so highly nonlinear that discrete load
steps are required for solution stability, which is the typical use case for
a Newtons Method solver.

#System requirements:

A computer running a 64 bit version of MacOSX or many other flavors of Unix.
The software was written and tested on an Ubuntu 12.10 64 bit machine.

An installation of the Trilinos agile components library must exist on the system
and you may have to modify 'allcompile.sh' in order get the filepaths right for 
the includes and links.
