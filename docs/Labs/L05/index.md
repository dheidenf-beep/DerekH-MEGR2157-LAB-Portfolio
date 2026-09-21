# A5 – Design a Snap fit

## Objective

The goal of the fifth lab was to design mathematically and 3D print a snap fit. The constraints for the snap fit was that it needed to be able to bend given a transverse force at the end of the flexure component of between 0.25 lbf and 5 lbf. The flexure is treated as a cantilever beam in this case with the force assumed to be at the free end of the flexure. The snap fit is required to hold a maximum axial force between 5 - 10 lbf. The shear stress from the axial load and the normal stress from the transverse load must not exceed the yield strength and ultimate shear strength of the material. The stress will be calculated using a safety factor of 3.5. 

## Research

### Printing Orientation



### Material Properties

The material I chose for the snap fit was PLA. Using the [data sheet from the MATWEB website](https://www.matweb.com/search/DataSheet.aspx?MatGUID=ab96a4c0655c4018a8785ac4031b9278&ckck=1), I used the lowest values for the yield strength, elastic modulus, and ultimate shear strength. This gave me a value of 8 MPa for the yield strength, 0.00232 GPa or 2.32 MPa for the elastic modulus, and 0.160 MPa for the ultimate shear strength. I calculated the maximum safe values for the yield strength and ultimate shear strength using the safety factor of 3.5. This gave me maximum values of 2.28 MPa for the maximum stress and 0.046 MPa for the ultimate shear strength. I used the beam bending equations for deformation and stress in the Machinery's Handbook.

**_INSRT SF WORK_**

## Calculations and CAD Parameters

### Calculations


## Snapfit Iteration 1



### Iteration 1 CAD Modeling



### Iteration 1 Preprocessing



### Iteration 1 Printing



### Iteration 1 Evaluation



## Snapfit Iteration 2



### Iteration 2 CAD Modeling



### Iteration 2 Preprocessing



### Iteration 2 Printing



### Iteration 2 Evaluation



## Lessons Learned



* [Snapfit Iteration 1 Download]()

* [Snapfit Iteration 2 Download]()



## Resources

Machinery's Handbook 32nd Edition

