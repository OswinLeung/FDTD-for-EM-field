
This repository documents my work on simulating the transmission of electromagnetic waves through a dielectric slab using the 1D Finite Difference Time Domain method(1D-FDTD) and 2D Finite Difference Time Domain method(2D-FDTD).

The purpose of this project is to explore how electromagnetic waves interact with materials of different permittivities and to calculate the transmission spectrum of the dielectric slab.

**1D - FDTD:**
Simulation Details

The simulation models a dielectric slab with a relative permittivity of ε_slab = 10, situated in a vacuum. The setup involves a Gaussian pulse modulated by a sine wave as an excitation source, and the fields are captured at a point beyond the slab to analyze transmission properties.

Key Parameters

	•	Wavelength (λ₀): 800 nm
	•	Slab thickness (d): 700 nm
	•	Spatial step (dx): Smaller than λ₀/20 for sufficient resolution
	•	Time step (dt): Calculated using the Courant condition

Objectives

	•	E_z Field Simulation: Record the electric field  E_z  inside and outside the slab over time.
	•	Transmission Spectrum Analysis: Use FFT to convert time-domain data to frequency-domain to understand how the slab affects different frequencies.
	•	Comparison with Theoretical Model: Compare the simulated transmission spectrum with theoretical predictions.

Repository Contents

	•	FDTD Simulation Code: Contains the implementation of the FDTD algorithm.
	•	Data Analysis Scripts: Scripts for performing FFT and analyzing the output data.
	•	Results: Plots and data files illustrating the simulation results.

**2D - FDTD:**
Simulation Details

The project simulates a square PEC cavity where electromagnetic waves are excited and their interactions within the cavity are studied. The simulation tracks the transverse magnetic (TM) modes, which consist of the  E_z ,  H_x , and  H_y  fields.

Parameters

	•	Wavelength (λ₀): 800 nm
	•	Cavity Dimensions: 800 nm x 800 nm
	•	Space Step (dx, dy): λ₀/20
	•	Time Step (dt): Derived using the Courant condition for stability

Objectives

	•	Field Simulation: Simulate  E_z ,  H_x , and  H_y  within the cavity.
	•	Mode Analysis: Use Fourier transforms to analyze the frequency and mode structures.
	•	Visualization: Provide visual output of the fields at resonance conditions.

 Repository Contents

	•	Simulation Code: Complete scripts for running the FDTD simulations.
	•	Analysis Scripts: Tools for performing Fourier analysis and extracting mode information.
	•	Results: Data and plots showing the field configurations and mode spectra.
	•	Documentation: Detailed explanation of the setup, theory, and interpretation of results.

Simulation Procedure

	1.	Initial Setup: Define the cavity geometry and material properties.
	2.	Source Excitation: Implement a sine wave envelope Gaussian pulse to excite the cavity.
	3.	Boundary Conditions: Apply PEC conditions to ensure reflective boundaries.
	4.	Field Recording: Capture the fields at specified probe locations.
	5.	Post-Processing: Use FFT to analyze the fields and identify resonant modes.
	6.	Visualization: Generate and display the field distributions for identified resonant modes.
