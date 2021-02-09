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
* **Fig 1.**: Mesh+snapshots
* Term to account for atmospheric pressure gradient caused by hurricane central depression + Wind stress parameterization taking saturation of wind drag for high wind speed. 

### Wave model

- Parallel Unstructured SWAN
  - $S_{in}$: Janssen parameterization for wind energy input term
  - $S_{ds}$: whitecapping (Komen) + bottom dissipation (Madsen) + depth-induced wave breaking
  -  $S_{nl}$: quadruplets interactions

- Wave forcings from WaveWatch III
- Depth-averaged Stokes drift can be computed by SWAN outputs

### Coupled model

- **Fig 2.** Roughness length for Madsen wave bottom dissipation is derived from SLIM bottom dissipation coefficient

  $z_0=H\exp\left[-\left(1+\dfrac{\kappa}{\sqrt{C_b}}\right)\right]$

## Comparison of trajectories

## Results

### Validation

* Validation of wind and pressure fields &rarr; **Fig 3**

* Validation of hydrodynamic outputs (elevation+currents) &rarr; **Fig. 4**

* Validation of wave outputs &rarr; **Fig. 5**

### Impact of waves

* Zones where difference in currents (with and without wave coupling) were the largest &rarr; **Fig. 6**

* We identified the zones with the largest differences in currents between SLIM and SLIM+SWAN during Irma. We then determined potential regions of origin for passive drifters that would reach these zones with large differences in current at the moment of the landfall of the hurricane in the Florida Keys. We then released passive virtual particles advected by SLIM and SLIM+SWAN currents from these origination regions and computed the distance between the centers of mass of the two clouds of particles through time. &rarr; **Fig. 7**

* Take-homme messages
  * The effect of waves on the currents is negligible before the passage of the hurricane. However, during the hurricane, it can produce differences of tens of km in a few hours in the position of particles transported by the currents.
  * When waves taken into account, particles stay on the shelf


## Discussion and conclusion

* Impact of Hurricane/waves on larval connectivity

* Impact of wave parameterization/boundary conditions on significant wave height gradient