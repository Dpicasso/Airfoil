# Airfoil
2-D analysis on Airfoil using FLUENT

# Summary

  This project will be analyzing a two dimensional profile of an airfoil using Ansys design modeler and Fluent solver. A velocity will be associated with the airfoil simulating flight and angle of attack will be varied to measure the change in pressure coefficients. The values will then be processed using linear regression and predictions can be made with the gathered data for a value of lift coefficient with specific angles of attack.
  
# Introduction

  I will be using Design Modeler and FLUENT solver in Ansys student version to calculate lift coefficients at different angles of attack, for simplicity, I will be analyzing only a 2-D Airfoil shape.
  
  Wings are one of the most important structures in aircraft structures. The special design of a wings profile, also known as the airofoil, is the main contributor to the ability of wings to create lift. There are many types of airfoil shapes and designs, and they all generate lift for their purpose. An aircraft that goes supersonic speeds will have a different design than a commercial plane. The idea of lift generation is an extremely complicated topic in itself, so I will not go into too much detail. There is two main theories of how lift is generated, there is the "Bernoulli" theory and the "Newton" theory. Now, Daniel Bernoulli nor Isaac Newton ever spent time to explain the theory of lift, but we use their ideas and equations to explain lift. Bernonulli theory states that as the velocity changes around the airfoil, pressure also changes. Summing up all the points of pressure across the area of the airfoil we get the aerodynamic forces applied to the profile. If we sum up all the points of velocity across the area it creates a turnring affect, and newtons third law states that for every action there is a reaction force in teh opposite direction. This force is applied onto the wing and theoretically creates lift. Both theories are correct but both contain error which we cannot use in applicable circumstances. 
  
  I want to use regression to create a predictive model for lift coefficients when changing the angle of attack. I want to solve fo rbest anlge of attack when taking off and landing, so at what angle of attack will the wings create the maximum ammount of lift.
