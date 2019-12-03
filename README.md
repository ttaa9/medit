# Medit [![Build Status](https://travis-ci.org/ISCDtoolbox/Medit.svg?branch=master)](https://travis-ci.org/ISCDtoolbox/Medit)
OpenGL-based scientific visualization software

Medit was developped to visualize numerical simulation results on unstructured meshes in two and three dimensions. Scalar, vector and tensor fields can be easily associated and displayed with meshes.

From [this repo](https://github.com/ISCDtoolbox/Medit) and described more [here](https://www.ljll.math.upmc.fr/frey/software.html) (including docs).

#### Installation

In a terminal, clone this repository:

   ` git clone https://github.com/ttaa9/medit.git `

   navigate to the downloaded directory:

   ` cd medit `

   then create build directory and compile the project using cmake
   ```
   mkdir build
   cd build
   cmake ..
   make
   make install
   ```

#### Usage

* Simply run :
    `medit yourFile.mesh`

* Usage help: 

   - Press `h` when the application is open to print usage

   - Add colour with `c` and change the background with `b`

   - `F1` turns on the clipping plane (and toggles it off)

   - `Right-click -> clipping -> toggle plane` controls whether to show the clipping plane or not (but clipping continues regardless)

   - `F2` toggles *control* of the clipping plane: use left-mouse to rotate and middle mouse to translate it

   - `Right-click -> File -> Hardcopy PPM` or pressing `H` generates a PPM-format image file (which can be viewed via e.g. `eog`).

   - To reverse the orientation of the clipping plane, do `right-click -> clipping -> inverse orient`

   - To "zoom"/scale/"move the camera in depth": use `alt+left-click`

### Acknowledgments

* Original repo [here](https://github.com/ISCDtoolbox/Medit)

* Thanks to C. Dobrzynski, there is an [inline HTML documentation](https://www.ljll.math.upmc.fr/frey/logiciels/Docmedit.dir/index.html) available in french.

* There is also a [technical report](https://www.ljll.math.upmc.fr/frey/publications/RT-0253.pdf) describing its main features.
