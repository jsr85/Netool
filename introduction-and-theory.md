# Introduction and Theory

Netool® is a steady-state completion and near-wellbore hydraulics simulator. It models flows from the reservoir through complex downhole completion strings to the wellhead.

Netool® helps well planning and completion design, as well as troubleshoots production problems and aids in taking appropriate corrective actions. The graphical user interface facilitates interactive well placement and easy selection of completion components, the effects of well position, length, and completion configuration on production and injection performance are easily modeled. Netool® replaces conventional [nodal analysis ](additional.md#nodal-analysis)software with the ability to model complex well hydraulics from sandface to the wellhead by combining reservoir deliverability with completion and vertical flow.

Netool models are:

* Full equation matrix 
* Black Oil Formulation with thermal module 
* Reservoir inflow calculated from reservoir grid data or logs 
* Simultaneous tubing and up to 4 annuli flows 
* Automatic solving of flow direction 
* Completion specific flow correlations

## Why do we need a detailed well simulator?

The convetional well simulation approach - [Nodal Analysis](additional.md#nodal-analysis) - was designed for vertical wells with a single [PI](additional.md#pi-productivity-index) zone with primary focus on Vertical Lift modeling and Artificial Lift optomization. But the industry is evolving rapidly of late.

The constant development of well drilling technologies allows the industry to develop more and more complex reservoirs.

![](.gitbook/assets/image%20%2836%29.png)

The development of drilling is followed by the development of completion technologies: Inflow Control Devices, Multilateral and Commingled Wells, Downhole Pressure sensors etc. are becoming increasingly common to see: 

![](.gitbook/assets/image%20%281%29.png)

New drilling and completion opportunities create new challenges for engineers: optimum long-term production performance depends on proper well and completion design and continuous evaluation. Multi-disciplined approach is required.

## Netool interface

The appliction consists of Netool Well Simulator \(or just Netool\) and Netool Simulation Results.

Netool Well Simulator is used for model building and simulation run. There are 4 tabs:

Reservoir & Well Trajectory - 

Global settings - 

Well Segments & Completions -

Fluid properties -  



![Netool input screen](.gitbook/assets/image%20%287%29.png)

![Well completion schematics](.gitbook/assets/image%20%2828%29.png)



Simulation Results 

![Netool Simulation Resilts](.gitbook/assets/image%20%2839%29.png)

Outputs:

* Total Well Rate – Oil, Water, Gas, GOR, WCT 
* IPR 
* Profiles along the length of the well:
  *  Tubing and annuli pressures 
  * Tubing and annuli flow rates 
  * Flow between annuli 
  * Flow into tubing 
  * Inflow from reservoir 
  * Permeability 
  * Reservoir pressure 
  * Productivity Index 
  * Velocities 
  * Skin 
  * Saturations \(or flowing fractions\)



User's well completion view:

![NETool has four completion strings](.gitbook/assets/image%20%2835%29.png)

Mathematical well completion representation:

![](.gitbook/assets/image%20%2822%29.png)

## Formats

.ntlcase file

.ntlplot

.ntlgrid

## What are the applications of Netool?

Netool is the software to design completion strings and accurately model well production based on reservoir properties. It brings together engineers from various disciplines: Completion, Drilling, Production, Reservoir and provides value for each discipline individually or in collaboratively. Here are some examples:

### Optimal well design, length and placement \(Drilling / Production / Reservoir\)

* Multi or single lateral? 
* Longer well has more reservoir contact but higher flow resistance losses too. What is the optimal well length? 
*  Well placement: near wellbore permeability greatly determines well productivity. Can we increase PI by moving trajectory slightly? 
* Drilling logs show very different results from seismic. Any idea what this well productivity will be? Maybe we can stop drilling earlier since we are behind the schedule and still meet production target?
* Smaller diameter – cheaper to drill. What will the impact of wellbore diameter on productivity be? 
* How much productivity we lose if we complete the well this way? 
* What will P10, 50 and 90 rates be for this well?

### Optimize completion design \(Completion\)

* Inflow Control Device settings must be tailored to reservoir properties found while drilling. 
* Inflow Control Valves must be designed for flow rate ranges of the zones they control and create minimal resistance when fully open. 
* Packers must withstand pressure difference between zones they separate and have enough length to minimize flow in near-well region around them. 
* Perforated cemented liners must be optimised for perforation shot density, diameter, phasing and orientation to achieve required skin factor. 
* Every slot in slotted liners costs money to make. How dense should they be? 
* Screens are expensive. Can we alternate them with blank pipes? 
* Do we need better screens because of high flow velocity?

### Combined Pump and Completion design \(Production\)

* Will this ESP fit my well?
* How much inflow from each part of the well I lose with a cheaper pump?
* Will this pump be sufficient until the end of production?
* We have 3 lower completion scenarios in mind and 3 pump candidates. What are the best well/pump pairs?
* The well has 3 valves with 10 settings each resulting in 1000 IPR curves. Is there an easy way to model it without generating these curves?

### Justify and design advanced wells \(Completion / Completion\)

* How can these completions modify well inflow profile? Do we really need to modify it? If yes – where and how much? 
* To what extend will advanced completions reduce GOR and WCUT when breakthrough occurs? 
* Do we need valves or ICD will work fine? 
* How many zones do we need in this well and where? 
* ICDs are expensive. How many do we really need? All manufacturers try to oversell. 
* ICDs are very different. Which one will work better for our hydrocarbon properties if every provider says his is the best one? 
* Do we need a custom valve ordered or the one from catalog is good? 
* How will advanced completions affect my acidizing?

### Address production problems \(Production / Reservoir\)

* How much should I reduce skin factor with acid to get back on target production? 
* What my P10, 50, 90 IPR will be for this stimulation job? 
* What will be the effect of stimulating some zones more than the others? 
* We have performed planned well clean-up but are not on target rate. What is the skin factor left? 
* If I block these fractures will matrix start to flow? 
* There are completions in my well. What my acid injection profile will be? 
* I suspect cross-flow or dumping. Reservoir simulator doesn’t show anything. Is there a more accurate wellbore simulator? 
* What should my valve settings be to avoid dumping?

### Troubleshoot poorly performing wells - PLT analysis \(Production / Reservoir\)

* My wells are at 90% WCUT. PLT shows where water mostly comes from. How much will I reduce it by recompletion or chemical treatment? 
* If we have logs and PLT can we detect completion failures? 
* PLT looks strange. Is there any soft I can put it in and understand the cause? 
* Since PLT can’t see flow in the annulus it gives a wrong inflow picture. Can any soft reconstruct reservoir inflow from tubing rate for us? 
* My high-rate gas well is not delivering. Is it due to well hydraulics or reservoir?

### What can you do with Netool: An example of Gas/Water Coning Control

Why should we care about inflow control?

![Horizontal well without Inflow Control Device](.gitbook/assets/image%20%2831%29.png)

![Horizontal well with Inflow Control Device](.gitbook/assets/image%20%2821%29.png)



Example of Coning Control - will ba added



