# SLIM+SWAN draft structure

## Introduction

Paragraph 1: wave-current interactions
1. Wave-current interactions play an important role in coastal areas
2. These interactions are complex and require a coupled model
3. Wave-currents interactions are more important in storm conditions 
4. Hurricane intensity and frequency in the GoM is expected to increase in the future &rArr; necessary to be able to model them accurately

Paragraph 2: lagrangian models
1. Lagrangian models are often used to model the transport of sediments, pollutants, larvae, etc.
2. Most of these models don't takes wave-current interactions into account (only Stokes drift)
3. This might generate significant errors under storm conditions &rArr; case study of Irma

Paragraph 3: Structure of the paper

## Methods

## Study area and data

Paragraph 1: Presentation of South Florida

Paragraph 2: Presentation of tide gauges, moorings and buoys

**Fig. 1**: Mesh + Hurricane track + bathymetry + measurement stations + zoom

### Wind and atmospheric pressure for Hurricane Irma

Paragraph 1
1. Some "fun facts" about Irma
2. Wind speeds obtained from HWind field
3. Construction of pressure field: ECMWF ERA-5 + Holland field using HURDAT 2

### Hydrodynamic model

Paragraph 1
1. Description of model equations
2. Saturation of wind drag coefficient

Paragraph 2: Mesh 

### Wave model

Paragraph 1
1. Description of model equations
2. Paramaterizations of different energy sources and sinks
3. Boundary conditions
4. Stokes drift

### Coupled model

Paragraph 1: To be developed 

**Fig 2.**: Model coupling (to be improved)

## Comparison of trajectories

Might have to rewrite this section

## Results

### Validation

Paragraph 1: Validation of atmospheric forcings
1. Constructed pressure field better at reproducing storm depression than ECMWF
2. Both HWind and ECMWF agree with observation but better timing/width of peak with HWind  

**Fig 3**: Reconstructed fields vs. measurements vs. ECMWF 

Paragraph 2: Validation of hydro
1. SSE agrees with observations and very good at reproducing storm surge
2. Fit especially good at Naples (both positive and negative surges)
3. Computation of correlation coefficient and veering angle at ADCP locations
4. Fit especially good for C10 (shallower)

**Fig. 4**: Modelled SSE & currents vs. measurements

* Validation of wave outputs &rarr; **Fig. 5**

### Impact of waves

Paragraph 1: Impact on currents
1. Significant differences > .5 m/s
2. Differences larger over reefs and between islands 

**Fig. 6** : Max differences in current velocities between SLIM and SLIM+SWAN

Paragraph 2: Impact on transport
1. Differences in trajectories of 10s of km
2. Particles tend to remain on the shelf when wave-current interactions taken into account
3. Importance of Stokes drift

**Fig. 7**: Comparison of trajectories SLIM vs. SLIM+SWAN+Stokes


## Discussion and conclusion

* Impact of Hurricane/waves on larval connectivity

* Impact of wave parameterization/boundary conditions on significant wave height gradient