#Date: 10-28-2013
#Author: Michael Brothers
#Title: Peridigm Complex Step Jacobian Archived Version

#Description: 

Contained in the compressed archive Peridigm_CS_Jacobian.tar.bz2
is a version of the Peridigm software modified to enable the use of the complex
step method to compute Jacobians when solving quasistatic problems. It is
written to produce experimental data of the kind presented in the companion
research paper and is best taken as a feasibility study rather than production
code.  

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

In order to run the code contained in the archive it is necessary
to extract the data to a directory of your choosing by typing: tar -xjvf
Peridigm_CS_Jacobian.tar.bz2 ./WhereIWantTheProgramToGo

Within the 'build' subdirectory of the Peridigm_CS_Jacobian directory is an
example cmake script to use to generate the make files needed to compile the
code. Refer to cmake user documentation for more directions, but naturally
specified file paths may differ for your system. 

#System requirements: 

Running the largest problem of the serial test series specified in the input
scripts and models directory requires at least 16GB of RAM. Running the
multicore test series specified in the same directory requires at least 1TB of
RAM and best done on an HPC cluster.
