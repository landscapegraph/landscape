# Landscape
A distributed graph sketching system that solves the connected components problem.

## How to Run Unit Tests on a Single Machine
### Operating System
This code has been tested on ubuntu-22,20, and 18. It will likely work on most linux based systems but these instructions apply to those OS's.
### Installation
 1. Install dependencies `sudo apt install git build-essential cmake openmpi-bin libopenmpi-dev`
 2. Clone this repository
 3. Create build directory under landscape dir. `mkdir landscape/build`
 4. Build project `cd landscape/build ; cmake .. ; cmake --build .`
### Run Unit Tests
To run the unit tests run the following command in the build directory. `mpirun -np 4 --oversubscribe ./distrib_tests`  
This commmand will run the unit tests using 4 local mpi processes.
