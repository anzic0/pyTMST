# pyTMST

Python port of the [MATLAB TMST toolbox](https://github.com/LeoVarnet/TMST) by
Léo Varnet. Currently a work in progress.

## Installation

0. (optional) It is recommended to install the dependencies in a virtual
   environment dedicated to your project.
   1. Create a virtual environment
      ```
      python3 -m venv <env-name>
      ```
   2. Activate the virtual environment
      ```
      source <env-name>/bin/activate
      ```

1. Clone repository
   ```
   git clone https://github.com/anzic0/pyTMST
   ```
2. Change into the local repository directory
   ```
   cd pyTMST
   ```
3. Install requirements
   ```
   pip install -r requirements.txt
   ```
4. Install package
   ```
   pip install .
   ```

## Testing

To run the test script, the following MATLAB toolboxes must be put in a directory
called ```matlab_toolboxes```:
- [TMST](https://github.com/LeoVarnet/TMST)
- [Auditory Modelling Toolbox](https://amtoolbox.org/)
- [YIN](http://audition.ens.fr/adc/sw/yin.zip)

Furthermore, the [MATLAB Engine API for Python](https://de.mathworks.com/help/matlab/matlab_external/install-the-matlab-engine-for-python.html)
corresponding to your local MATLAB version needs to be installed. For this, the
following steps may be followed:

1. Find the root directory of your MATLAB installation by running
   ```
   matlabroot
   ```
   in MATLAB
2. Change into the following subdirectory of the MATLAB root
   ```
   cd <matlab-root>/extern/engines/python
   ```
3. Install via pip
   ```
   python -m pip install .
   ```
