# FDTD-for-EM-field

Overview

This repository contains the implementation of the 1D Finite Difference Time Domain (FDTD) method, as outlined in specific academic coursework. The simulation investigates the propagation of electromagnetic waves through a discretized space under various conditions and boundary types.

Features

	•	Implementation of the 1D FDTD algorithm.
	•	Use of Perfect Electric Conductor (PEC) and absorbing boundary conditions.
	•	Three different excitation functions:
	•	DC Gaussian
	•	Continuous Wave (CW) Sinusoid
	•	Sine Envelope Gaussian
	•	Visualization of electric (E) and magnetic (H) fields over time.

Parameters

The simulations run with the following parameters:

	•	Permittivity and Permeability of free space.
	•	Speed of light in vacuum.
	•	Center frequency of 1 GHz.
	•	Spatial domain discretized into 500 cells.

Excitation Functions

DC Gaussian

Characterized by its width and centered around a specified time point, affecting the profile of the propagated wave.

CW Sinusoid

A continuous wave that helps in observing the steady-state behavior of the system.

Sine Envelope Gaussian

Combines a sinusoidal function with a Gaussian envelope for localized wave propagation analysis.

Boundary Conditions

	•	PEC Boundary: Simulates a perfect electric conductor at the domain boundaries.
	•	Absorbing Boundary: Implements absorbing conditions to minimize reflections.
