# CPMD-ttotshort
ttotshort is a little program that takes the trajectory output file from CPMD and keeps only the listed atoms. The ttotshort.in (input) file has the following structure:

#####
TRA3      -> File name. This can be TRA(N°) or any trayectory file created with ttotcenter
102       -> Total atoms in the cage.
          -> Optional empty line
1         -> Atomic labels as you see in molden. It does not matter the order
2
3
31
32
33
34
35

        -> As a suggestion you can put each molecule labels separated by an empty line. These lines will not be read
22
93
94

26
98
#####

To execute it you need the files ttotshort.py (program) and ttotshort.in (input) in the working folder and write in the command line:

$ python ttotshort.py

or:

$ python3 ttotshort.py

The output file will have the same name as the input, adding "short" at the end (e.g. TRA3 -> TRA3short). If you have any problem, please contact me at alvarez@theochen.uni-hannover.de attaching the trajectory file.
Enjoy!

Luis Álvarez
