# LandScape
A distributed graph sketching system that solves the connected components problem.

## How to Run Unit Tests on a Single Machine
### Operating System
This code has been tested on ubuntu-20 and ubuntu-18. It will likely work on most linux based systems.
### Installation
 1. Clone this repository
 2. Install dependencies `sudo apt install git gcc-c++ cmake openmpi-bin libopenmpi-dev`
 3. Create build directory under landscape dir. `mkdir landscape/build`
 4. Build project `cd landscape/build ; cmake .. ; cmake --build .`
 
### Run Unit Tests
To run the unit tests run the following command in the build directory. `./distrib_tests`
