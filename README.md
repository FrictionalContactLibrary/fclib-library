fclib-library repository
========================

## A open collection of frictional contact problems

<div align="center">
        <img height="250px" src="./Local/LMGC90/Aqueduct_PR/Aqueduc_PR.png" alt="About screen" title="Aqueduct.png"</img>
        <img height="250px" src="./Local/LMGC90/Bridge_PR/Bridge_PR_1.png" alt="About screen" title="Bridge_PR_1.png"</img><br/>
        <img height="200px" src="./Local/siconos/Chain/Chains.png" alt="About screen" title="Chains.png"</img>
        <img height="200px" src="./Local/siconos/BoxesStack/BoxesStack2.png" alt="About screen" title="BoxesStack2.png"</img>
        <img height="200px" src="./Local/siconos/Chute_local_problems/Chute_1000_light.jpg" alt="About screen" title="BoxesStack2.png"</img>
        <img height="200px" src="./Local/siconos/KaplasTower/KaplasTower.png" alt="About screen" title="BoxesStack2.png"</img>
        <img height="200px" src="./Local/LMGC90/100_PR_PerioBox/100_PR_PerioBox.png" alt="About screen" title="100_PR_Periobox.png"</img>
        <img height="200px" src="./Local/LMGC90/945_SP_Box_PL/945_SP_Box_PL.png" alt="About screen" title="945_SP_Box_PL.png"</img>
        <img height="200px" src="./Local/LMGC90/Cubes_H8/Cubes_H8_5.png" alt="About screen" title="Cubes_H8_5.png"</img>
        <img height="200px" src="./Local/LMGC90/LowWall_FEM/LowWall_FEM.png" alt="About screen" title="LowWall_FEM.png"</img>
        <img height="500px" src="./Local/siconos/Chute_1000/Chute_1000_4x.png" alt="About screen" title="Chute_1000_4x.png"</img>
</div>


This repository contains the problem files of the fclib library. 

The hdf5 file can be read with the fclib API in C or in Python. The code can be found at [FrictionalContactLibrary/fclib](https://github.com/FrictionalContactLibrary/fclib)

More information is avalaible on the [website of the fclib project](https://frictionalcontactlibrary.github.io/index.html)


What is fclib ?
---------------
fclib is
 * an open source collection of Frictional Contact (FC) problems stored in a specific HDF5 format,
 * an open source light implementation of Input/Output functions in C Language to read and write problems.
 
The goal of this work is to set up a collection of 2D and 3D Frictional Contact (FC) problems in order to
 * set up a list of benchmarks,
 * provide a standard framework for testing available and new algorithms,
 * share common formulations of problems in order to exchange data.

What is a Frictional contact problem ?
--------------------------------------

A Frictional contact problem is algebraic problem obtained after possible time and space discretizations of problems
of mechanics of solid involving contact and Coulomb's friction. The mathematical structure of the problem is 
a second-order cone complementarity problem. For more details, you could have a look to the fclib specifications in

Vincent Acary, Maurice Brémond, Tomasz Koziara, Franck Pérignon. 
FCLIB: a collection of discrete 3D Frictional Contact problems. 
[Technical Report] RT-0444, INRIA. 2014, pp.34. <hal-00945820v2>
https://hal.inria.fr/hal-00945820v2/document

git lfs
-------
It uses git lfs  for the versioning and the cloning. By using git sparse-checkout system, you can clone only what you need.


