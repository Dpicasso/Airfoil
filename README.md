# Airfoil
2-D analysis on Airfoil using FLUENT

# Summary

  This project will be analyzing a two dimensional profile of an airfoil using Ansys design modeler and Fluent solver. A velocity will be associated with the airfoil simulating flight and angle of attack will be varied to measure the change in pressure coefficients. The values will then be processed using linear regression and predictions can be made with the gathered data for a value of lift coefficient with specific angles of attack.
  
# Introduction

  I will be using Design Modeler and FLUENT solver in Ansys student version to calculate lift coefficients at different angles of attack, for simplicity, I will be analyzing only a 2-D Airfoil shape.
  
  Wings are one of the most important structures in aircraft structures. The special design of a wings profile, also known as the airofoil, is the main contributor to the ability of wings to create lift. There are many types of airfoil shapes and designs, and they all generate lift for their purpose. An aircraft that goes supersonic speeds will have a different design than a commercial plane. The idea of lift generation is an extremely complicated topic in itself, so I will not go into too much detail. There is two main theories of how lift is generated, there is the "Bernoulli" theory and the "Newton" theory. Now, Daniel Bernoulli nor Isaac Newton ever spent time to explain the theory of lift, but we use their ideas and equations to explain lift. Bernonulli theory states that as the velocity changes around the airfoil, pressure also changes. Summing up all the points of pressure across the area of the airfoil we get the aerodynamic forces applied to the profile. If we sum up all the points of velocity across the area it creates a turnring affect, and newtons third law states that for every action there is a reaction force in teh opposite direction. This force is applied onto the wing and theoretically creates lift. Both theories are correct but both contain error which we cannot use in applicable circumstances. 
  
  I want to use regression to create a predictive model for lift coefficients when changing the angle of attack. I want to solve fo rbest anlge of attack when taking off and landing, so at what angle of attack will the wings create the maximum ammount of lift.
  
# Procedure
  The first step was to create the geometry of an airfoil. Luckily the internet has plenty of recources to get data points for you to import into desgin modeler. I foil an airofil calculator that allowed you to creaet your own airofil profile, I used a premade airfoil NACA0012. I chose thise profile becuase it was the most simple and was also symmetrical, so I only have to measure the airofil rotating in one direction. A geometric volume was then created to simulate an atmosphere.
  
  The next step was to create a mesh around the airfoil. Since a dynamic mesh is needed to simulate the airfoil rotating two mesh faces were used. The inner mesh will be passive as the outer mesh will be deforming. The most difficult part of this simmulation was creating the dynamic mesh. There were recources to look online, but every person seemed to do it their own way. Through a lot of trial and error I was able to create a mesh that rotated from 0 degrees to 20 degrees. I used Ansys to calculate lift coefficients and record the values for each of the 100 time steps. 
  
  The last step is the statistical analysis. Taking the lift coefficeint data from Fluent I can import and process the data in python. We first want to pre process the data first. This will make the columns have zer mean and unit varience. The data will be centered at zero and the scales of the values will not be scattered. We then apply a linear model with multiple polynomial terms. Using a set of training data and test data and see how well our model can predict the lift coefficient with a given angle of attack values.
  
# Results

![Alt text](relative/path/to/img.jpg?raw=true "airfoil sketch")
