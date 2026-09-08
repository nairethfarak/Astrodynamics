# Astrodynamics 
This repository contains a collection of academic assignments developed for the Astrodynamics course, covering orbital mechanics, propulsion, orbital maneuvers, perturbation analysis, interplanetary trajectories, and Earth–Moon mission design.

The projects were developed primarily in Python, using numerical simulation, analytical methods, and astrodynamics libraries such as REBOUND, SPICE, NumPy, SciPy, and Matplotlib.

## Projects

### 1. Multistage Rocket Performance
*File:* Multistage_Rocket_Performance.ipynb

Analysis of the performance and mass distribution of a three-stage launch vehicle.

The project includes:

- Payload and structural mass fractions.
- Stage mass ratios.
- Total $\Delta v$ estimation.
- Propellant, structural, and initial mass calculations for each stage.
- Analysis of $\Delta v/c$ as a function of structural efficiency and number of stages.
- Comparison with reference results from the literature.

### 2. Orbital Maneuvers

*File:* Orbital_Maneuvers.ipynb

Analysis and numerical simulation of classical orbital transfer maneuvers.

The project covers:

Hohmann transfer
Coaxial transfer
Bi-elliptic transfer
Phasing maneuver

For each maneuver, orbital velocities, $\Delta v$, transfer times, propellant requirements, and orbital trajectories are calculated and analyzed.


### 3. Orbital Propagation and Atmospheric Drag
*File:* Orbital_Propagation_Atmospheric_Drag.ipynb

Analysis of the evolution of a terrestrial orbit under propulsive maneuvers and atmospheric drag.

The project includes:

- Impulsive and finite-duration maneuvers.
- Variable spacecraft mass and thrust modeling.
- Cowell's method for orbital propagation.
- Atmospheric density modeling using ussa1976.
- Calculation of ballistic coefficient and relative atmospheric velocity.
- Comparison of Euler, Leap-Frog, and Radau numerical integration methods.
- Analysis of the evolution of apogee and perigee during orbital decay.
- 3D visualization of spacecraft trajectories.

### 4. Earth's Gravitational Perturbations
*File:* Earth_Gravitational _Perturbations

Study of orbital perturbations caused by the non-spherical gravitational field of the Earth.

The project implements the EGM96 gravitational model and analyzes the effects of Earth's gravitational harmonics.

It includes:

- Extraction of zonal harmonics from $J_2$ to $J_6$.
- Efficient computation of perturbing accelerations using Numba.
- Orbital propagation using REBOUND.
- Isolated analysis of the $J_2$ perturbation.
- Implementation of Gauss' planetary equations.
- Comparison between analytical perturbation models and numerical propagation.
- Analysis of changes in $a$, $e$, $i$, $\Omega$, and $\omega$.


### 5. Gravitational Perturbations & Solar Geometry
*File:* Gravitational_Perturbations_Solar_Geometry.ipynb

Extended analysis of gravitational perturbations and spacecraft orbital dynamics.

The project includes:

- EGM96 spherical harmonic gravitational modeling.
- Comparison between $J_2$-only and higher-order harmonic models.
- Numerical propagation using REBOUND.
- Secular variations of classical orbital elements.
- Symbolic calculation of secular orbital-element rates using SymPy.
- Analysis of nodal regression and periapsis precession.
- Solar position determination using SPICE.
- Transformation between ecliptic and equatorial reference frames.
- Geometric determination of spacecraft illumination conditions.
- Orbital propagation of the Hinode satellite using TLE and SGP4 data.

### 6. Gauss Planetary Equations & Third-Body Perturbations
*File:* Gauss_Equations_Third_Body_Perturbations.ipynb

Analysis of orbital perturbations using Gauss' planetary equations, with numerical comparisons against REBOUND propagation.

The project covers:

- Earth's $J_2$ perturbation.
- Numerical integration of Gauss' equations.
- Comparison between Gauss and REBOUND solutions.
- Solar radiation pressure.
- Atmospheric density modeling.
- Comparison between solar radiation pressure and atmospheric pressure.
- Lunar gravitational perturbations.
- Solar gravitational perturbations.
- Long-term orbital propagation and analysis of orbital-element variations.

### 7. Earth Escape & Heliocentric Transfer
*File:* Earth_Escape_Heliocentric_Transfer.ipynb

Analysis of the transition from a hyperbolic Earth-centered escape trajectory to a heliocentric orbit.

The project includes:

- Initial heliocentric orbital state determination.
- Orientation of the hyperbolic Earth escape trajectory.
- Calculation of true, eccentric, and mean anomalies.
- Time required to reach the Earth's sphere of influence.
- Orbital propagation using spiceypy.prop2b.
- Calculation of heliocentric orbital elements.
- Analysis of escape velocity, circular velocity, and $\Delta v$.
- Comparison between SPICE and REBOUND propagation results.
- Visualization of Earth-escape and heliocentric trajectories.

### 8. Earth–Jupiter Transfer & Gravity Assist
*File:* Earth_Jupiter_Gravity_Assist.ipynb

Analysis of an Earth-to-Jupiter transfer using a Hohmann-type trajectory and gravity-assist maneuver.

The project calculates:

- Initial and transfer orbit parameters.
- Jupiter's orbital velocity.
- Hyperbolic excess velocity relative to Jupiter.
- Flyby trajectory eccentricity.
- Gravity-assist turning angle.
- Post-flyby velocity and required $\Delta v$.
- Final orbital angular momentum.
- Final semi-major axis and eccentricity.
- Parametric analysis of $\Delta v/v_\infty$ for different eccentricities.

### 9. Earth–Moon Transfers
*File:* Earth_Moon_Transfers.ipynb

Analysis of different strategies for transferring a spacecraft from Earth to the Moon.

The project includes:

- Lunar orbital analysis using SPICE data.
- Transformation between ECLIPJ2000 and J2000 reference frames.
- Hohmann-like Earth–Moon transfer from a 320 km parking orbit.
- Calculation of transfer orbit parameters and flight time.
- Faster Earth–Moon transfer trajectories.
- 3D mission simulations using REBOUND.
- Comparison of Hohmann and faster transfers.
- Analysis of an Artemis II mission scenario.
- Parametric analysis of initial velocity versus flight time and total $\Delta v$.















