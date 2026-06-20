# Nonlinear-Finite-Element-Analysis-of-a-2D-plate-with-a-central-hole-under-uniform-traction

## 2.2 Running the Code

To run the code and analyse the behaviour of the two-dimensional plate with a central hole under uniform traction, follow these steps:

1. Download or clone the complete repository and save all MATLAB files, built-in function files, mesh files, and the element routine in the current working directory.

2. Open the project folder in MATLAB.

3. Set the MATLAB working directory to the folder where the code files are saved. This can be done using the **Current Folder** panel in the MATLAB interface.

4. Open the file `main_routine.m`. The main input parameters can be modified according to the required analysis case:

   - Young’s modulus, `E`: 210 GPa  
   - Poisson’s ratio, `nu`: 0.3  
   - Initial yield stress, `sigmaY`: 0.2 GPa  
     - For linear elastic deformation, set `sigmaY = E`.
   - Linear isotropic hardening modulus, `hard_iso`: 1.0 GPa  
   - Increase in yield stress due to exponential hardening, `deltaY`: 0.0 GPa  
   - Shape parameter for exponential hardening, `h_sh`: 15  
   - Linear kinematic hardening modulus, `hard_kin`: 0.0 GPa  

5. These parameters are already preset in the `main_routine.m` file. They can be changed depending on the user-specific requirements.

6. The code allows the user to select the desired mesh profile by uncommenting the corresponding mesh section in `main_routine.m`. This provides flexibility for analysing different mesh refinements.

7. After assigning the required input parameters, run the program by typing the following command in the MATLAB Command Window:

   ```matlab
   main_routine
