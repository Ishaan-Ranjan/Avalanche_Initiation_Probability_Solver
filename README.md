# Avalanche_Initiation_Probability_Solver
This repo contains code that uses the shooting method to solve a system of differential equations relating to Avalanche Initiation Probability. Newton's method is also used to improve the guess for initial conditions.

The code works by using the Finite Differences Method to generate a list of values for each function (P_e and P_h). The shooting method is used because the two boundary condition given - P_e(0) = 0 and P_h(W) = 0 - are difficult to use, since they both are from different x values. Instead, we guess P_h(0), and then complete FDM in order to check whether P_h(W) ended up being close to 0. If the end result is too far, Newton's method is used the improve the guess.

The equations used are from the paper "Triggering Phenomena in Avalanche Diodes" by Oldham et. al.

<img width="373" height="208" alt="Screenshot 2026-07-09 at 3 09 54 PM" src="https://github.com/user-attachments/assets/097d4062-71d0-426f-b17a-70798b9bdc36" />
