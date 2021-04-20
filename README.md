# SLIM+SWAN draft structure

## 1. Introduction

1. Tropical cyclones more and more frequent/intense &rArr; understanding wave-current interactions is important

2. Wave-current interactions are complex &rArr; need coupled model

3. Complex topology in coastal areas &rArr; need unstructured model

4.  Wave-current interactions rarely taken into account when studying transport of passive drifters

5. Objective of study = assess impact of wave-current coupling when studying transport during Hurricane Irma + Structure of paper

## 2. Methods

#### 2.1. Study area and observational data

1. Description of South Florida +Tropical cyclones in Florida/Gulf of Mexico

2. Description of observational data &rarr; [ **Fig. 1B** ]
    - tide gauges &rarr; sea surface elevation
    - ADCP &rarr; currents 
    - buoys &rarr; waves

#### 2.2. Wind and atmospheric pressure for Hurricane Irma

1. Description of Irma and data used for wind and pressure
    - Information about Irma
    - Wind speed: HWind data set + combination with ERA-5 &rarr; [ **Fig. 2A** ]
    - Atmospheric pressure: construction of Holland profile using HURDAT + combination with ERA-5 &rarr; [ **Fig. 2B** ]

#### 2.3. Hydrodynamic model

1. Description of model equations + forcings  &rarr; [ eq. 1 ]

2. Saturation of wind drag coefficient &rarr; [ eqs. 2-4 ]

3. Description of mesh &rarr;  [ **Fig. 1A+C** ]

#### 2.4. Wave model

1. Description of model equations
    - Action balance equation &rarr; [ eq. 5 ]
    - Spectral discretization
    - Model parameterization
    - Boundary conditions

2. Stokes drift: definition + equations &rarr; [ eq. 6 ]

#### 2.5. Coupled model

1. Mathematical description of coupling
    - Mention vortex-force representation

2. Numerical implementation of coupling &rarr; [ **Fig 3.** ]

#### 2.6. Quantifying the effect of wave-current interactions on transport

1. Description of approach
    - Initial positions of particles using backtracking &rarr; [ **Fig. 4** ]
    - Description of different sets of currents

## 3. Results

1. Plan of the section &rarr; [ **Table 1** ]

#### 3.1. Model validation

1. Validation of atmospheric forcings &rarr; [ **Fig. 5**]
    - Hybrid fields better reproduce field measurements

2. Validation of hydrodynamic outputs
    - Amplitude and timing of storm surge well reproduced &rarr; [ **Fig. 6** ]
    - Modeled currents agree well with ADCP, especially in shallow region &rarr; [ **Fig. 7** ]

3. Validation of wave outputs
    - Good agreement with observed SWH (better on WFS) &rarr; [ **Fig. 8** ]

#### 3.2. Impact of waves on currents and transport

1. Impact of wave-current interactions on current velocity &rarr; [ **Fig. 9** ]
    - Differences of up to 1 m/s, with SLIM+SWAN > SLIM
    - Differences stronger on shelf break and in region where wind stress stronger

2. Impact of waves on modeled trajectories &rarr; [ **Fig. 10A**]
    - Differences > 5 km due to wave-current interactions
    - Differences larger on outer shelf + require more time to stabilize

3. Impact of Stokes drift &rarr;  [ **Fig. 10A+B** ]
    - Stokes drift has larger effects than radiation-stress gradient (similar on outer shelf during the passage of Irma)
    - Impact of radiation stress gradient alone only significant during passage of hurricane
    - Difference between coupled and uncoupled Stokes drift negligible 

## Discussion

1. Take home messages:
    - SLIM+SWAN correctly reproduces both the hydrodynamics and wave dynamics during hurricane Irma but it requires good atmospheric forcings and good wave parametrization
    - The additional wave stress can locally increase the current amplitude by about 1 m/s, which could be even more if it was not strongly dissipated by the coral reefs along the outer shelf that act as a very efficient coastal defense.
    - Transport processes during heavy-wind events are influenced by the wave coupling but the Stokes drift dominates the wave-currents interactions. 

2. Model reproduced well storm surge
    - Important as most damages during Irma caused by surge (+ high resolution of model) 
    - Impact of negative surge

3. Importance of wave parameterization and model resolution when modeling wave-current interactions during tropical cyclone
    - Current-wave interaction in Gulf Stream
    - Spectral and spatial resolution + boundary conditions
    - Parameterization chosen for whitecapping and wind growth &rArr; better wave results on WFS

4. Impact of coral barrier
    - Strong wave dissipation &rArr; large radiation stress gradient &rArr; large impact on current velocity
    - Differences between inner and outer shelf due to sheltering

5. Stokes drift has larger impact than radiation stress gradient + coupled stokes drift pretty similar to uncoupled stokes drift &rArr; can neglect wave coupling in shallow sheltered regions in fair weather


## Conclusion

1. Summary of paper

2. Limitations of model
    - Wind-wave interactions
    - Calibration of wave model parameters

3. Conclusion (add cheap approach as in OpenDrift ?)
