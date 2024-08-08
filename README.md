# MSRE_Dynamics-Xenon
The repo for the coupled model of MSRE. Refer to 10.1016/j.anucene.2024.110705 and 10.1016/j.anucene.2024.110525 for general information on the model structure. 

Usage:
1. Run the initialization *.mlx file for the desired fuel type. Change the parameters if needed.
2. Note that the default running mode is Accerlerator, which requires the MinGW-Win64 compiler on Windows. Check https://www.mathworks.com/matlabcentral/fileexchange/52848-matlab-support-for-mingw-w64-c-c-fortran-compiler for how to set it up.
3. Check the relavent blocks in the model to make sure the Varient blocks are setup properly for the type of simulation performed. Add or change the signal storage based on the intended use. The model does not log all the information during simulation.
4. Use the processingSpecturm.mlx file to run the simulation. Note that a initialization run is required before running subsequent codes to obtain the frequency response. Remember the initial state can't be used if any physical parameters are changed. You'll have an error.

Note:
Only one version of the model is uploaded to avoid confusion, which is setup for frequency analysis. Other types of usage can be easily setup by slightly changing the model.
