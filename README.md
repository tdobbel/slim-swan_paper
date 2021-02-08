# SLIM+SWAN draft structure

## Introduction

* Importance of interactions between waves and currents in storm conditions
* Transports phenomenons important in region of the FRT: larvae and oil (cite Matthieu's paper) &rArr; link to connectivity study (reproduction period of coral during season of hurricanes)

## Methods

### Wind and atmospheric pressure for Hurricane Irma

- Wind speeds are obtained from H*Wind field data

- Pressure field is obtained by combining ECMWF model outputs with Holland profile based on HURDAT hurricane track

  $p(r) = p_c + (101330-p_c)\exp(-\frac{r_\text{mws}}{r})$

### Hydrodynamic model

* Barotropic version of the unstructured-mesh ocean model SLIM ([www.slim-ocean.be](http://www.slim-ocean.be)). 
* **[FIGURE]** Mesh of the computational domain with snapshots of simulated instantaneous currents and significant wave height on 2017-09-10 at 11:00:00. The mesh resolution ranges from 100 m in the Florida Keys to a maximum of 10 km offshore. 
* Term to account for atmospheric pressure gradient caused by hurricane central depression + Wind stress parameterization taking saturation of wind drag for high wind speed. 

### Wave model

- Parallel Unstructured SWAN
  - $S_{in}$: Janssen parameterization for wind energy input term
  - $S_{ds}$: whitecapping (Komen) + bottom dissipation (Madsen) + depth-induced wave breaking
  -  $S_{nl}$: quadruplets interactions

- Wave forcings from WaveWatch III
- Depth-averaged Stokes drift can be computed by SWAN outputs

### Coupled model

- Roughness length for Madsen wave bottom dissipation is derived from SLIM bottom dissipation coefficient

  $z_0=H\exp\left[-\left(1+\dfrac{\kappa}{\sqrt{C_b}}\right)\right]$

## Results

### Validation

* **[FIGURE] ** The atmospheric forcings have been validated with meteorological station observations at Vaca Key. The reconstructed atmospheric pressure and wind speed agree well with field measurements

* **[FIGURE] ** The sea-surface elevation produced by the coupled wave-current model agrees with SSE and current velocity observations at different stations. The fit is particularly good in the Florida Keys and in Naples, on the inner Florida shelf. The coupled model currents have been validated against current meter data on the inner Florida shelf. The current speed and direction during the hurricane agrees well with the observations.
* **[FIGURE] ** The significant wave height produced by the coupled model has been compared to buoy measurements at 4 different stations. The timing and amplitude of the peak during the hurricane is correctly reproduced for all stations. For station 42036, the period and direction of the waves also agree well with observations.

### Impact of waves

* **[FIGURE] ** Maximum of the difference between SLIM and SLIM+SWAN currents speed between 2017-09-07 00:00:00 and 2017-09-13 00:00:00. The difference between the coupled and uncoupled model, which represents the effect of the wave-induced stress, can yield differences of 0.5 m/s in the simulated currents during the passage of the hurricane. SLIM+SWAN currents velocities are larger than the currents modeled by SLIM alone  
* **[FIGURE]** We identified the zones with the largest differences in currents between SLIM and SLIM+SWAN during Irma. We then determined potential regions of origin for passive drifters that would reach these zones with large differences in current at the moment of the landfall of the hurricane in the Florida Keys. We then released passive virtual particles advected by SLIM and SLIM+SWAN currents from these origination regions and computed the distance between the centers of mass of the two clouds of particles through time.
* **[FIGURE]** Comparison of passive drifters trajectories with SLIM+SWAN+Stokes drift vs. SLIM alone. A snapshot of the positions of the particles released from region 2 is shown after the passage of Irma in the Florida Keys. Particles advected by the currents of the coupled model tend to remain on the shelf while particles advected by SLIM alone are mostly transported along the shelf break.
* The effect of waves on the currents is negligible before the passage of the hurricane. However, during the hurricane, it can produce differences of tens of km in a few hours in the position of particles transported by the currents. . 

## Discussion and conclusion