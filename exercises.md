# Exercises

## “My first well”

Import Reservoir Model. 

* Choose File -&gt; Open/Create Well case
* Switch to the “Open/Create Well Case” page
* Press “Add Reservoir model”

![](.gitbook/assets/image%20%2832%29.png)

![](.gitbook/assets/image%20%2813%29.png)



Select input data format

* Select ”Import reservoir model in Eclipse format”
* Push ”Next &gt;”

![](.gitbook/assets/image%20%2825%29.png)

Import files

* Browse to find the Eclipse INIT file 
* Select the file ’long horizontal.INIT’  
* Push ”Next &gt;” 
* NETool lists all Eclipse files with the same name. 
* Push ”Next &gt;” twice

![](.gitbook/assets/image%20%2818%29.png)

![](.gitbook/assets/image%20%283%29.png)



* Select all timesteps
* Push ”Next &gt;”
* Set the name of Imported Reservoir Model 
* Press ‘Finish’

![](.gitbook/assets/image%20%2817%29.png)



* Choose ‘Create a new well case’ 
* Press OK

![](.gitbook/assets/image%20%285%29.png)



* Go to Reservoir & Well Trajectory tab 
* Click several points on the upper reservoir view

![](.gitbook/assets/image%20%2819%29.png)



* Select ‘Global Settings’ tab at the top of main window. 
* Choose ‘Well Target & IPR’ folder in Global Settings. 
* Set Bottomhole pressure = 100 bar, and choose ‘BHP defined at bottomhole MD’.

![](.gitbook/assets/image%20%2841%29.png)

! Please note that for MD = 0, TVD ≠ 0, that’s why bottomhole point here. Netool allows modelling of the entire well: simply change the well survey with TVD at the depth of the wellhead \(MD = 0\).



* Go to ‘Well Segment & Completion’ tab 
* ‘Drill’ the well creating 10 segments of the same length 
* Press ‘Create’

![](.gitbook/assets/image%20%2811%29.png)



* Press “Run Simulation” button

![](.gitbook/assets/image%20%289%29.png)



* Interpret Results

![](.gitbook/assets/image%20%2820%29.png)

## Build Case from Scratch with a “Wizard”

Well Description:

* See figure below
* Vertical Producer 
* Screens completion 
* Oil Flowrate Target = 3000 stb/day 
* 2 geological zones with different permeabilities 
* Initially 80% oil saturation 
* RelPerm – Wyllie’s correlations for cemented sandstone 
* PVT - Undersaturated oil and water 
* Reservoir Flow Modeling 
  * Steady-State 
  * Drainage radius = 2000 ft 
  * Supplied reservoir pressure = Average reservoir pressure 
  * Add hydrostatic correction to entered reservoir pressure

![](.gitbook/assets/image%20%2837%29.png)

Follow the instructions.



### Get Started with Netool Wizard

Click File -&gt; Create from Wizard...

![](.gitbook/assets/image%20%2814%29.png)

### Create New Project

![](.gitbook/assets/image%20%2823%29.png)



### Well Trajectory

* Enter coordinates for Top and Bottom 
* Enter Measured depth of Heel 
* Click “Commit” button

![](.gitbook/assets/image%20%2840%29.png)

### Well Segmentation

* Switch to Well Segments & Completion tab on the top of main NETool window 
* Enter four ‘Segments MD’ values to define segment boundaries for 3 segments 
* Click “Commit” button

![](.gitbook/assets/image%20%2826%29.png)

### General Specs

* Choose Well type Producer 
* Select phases Oil and Water

![](.gitbook/assets/image%20%2838%29.png)

### Well Target and IPR

* Open Global Settings Select “Well Target & IPR” folder 
* Choose “Single target” 
* Define production well target: Oil Flowrate = 3000 stb/d

![](.gitbook/assets/image%20%284%29.png)

### Reservoir Flow

* Set Reservoir Pressure = Hydrostatics from bottomhole MD 
* Set Reservoir Pressure Value = 5000 psi 
* Choose Radial inflow model and Steady Radial PI Model type 
* Choose Average pressure in drainage area mode

![](.gitbook/assets/image%20%288%29.png)

### PVT Properties

* Accept default values and choose Oil PVT tab 
* Enter constant solution gas-oil ratio \(Rs\) of 100 SCF/STB 
* Define oil phase formation volume factor \(Bo\), viscosity as function of pressure

![](.gitbook/assets/image%20%2834%29.png)

### Relative Permeabilities and Well Case Name

* Choose Wyllie’s consolidated sandstone correlation for RelPerm modelling
* Save the wellcase by giving it a name

![](.gitbook/assets/image%20%2810%29.png)

Wizard is finished !! 

Further defintion of reservoir properties and completion parts is performed in the Well Segment Settings & Completions panel. It is also possible to return to previous menus to revise supplied data.



### Hole & Completion

* Select Well Segments & Completions panel 
* Choose folder Hole & Completion
* In column Sand Control select “Screen“ for all segments
* Choose folder Diameters 
* Define the Wellbore Diameter = 9 in column Wellbore Diameter\*

\*Differs from well schematic diagram

![](.gitbook/assets/image%20%2833%29.png)

### 

### Permeability

* Choose folder Reservoir Parameters 
* Choose folder Permeability 
* In column Kh define permeability for segments 1, 2 = 200 mD and segment 3 = 1000 mD

![](.gitbook/assets/image%20%2824%29.png)



### Saturation and Skin

* Choose folder Saturations \(Reservoir Parameters-&gt;Mobility/Saturations-&gt; Water Saturation\) 
* In column Water Saturation define value = 0.2 for all segments. This calculate the Oil Saturation column to be 0.8 
* The reservoir doesn’t have damage, so, in Skin panel, leave checkbox Near Wellbore Damage unselected for all segments. Set Additional Skin for all segments as 0.

![](.gitbook/assets/image%20%2812%29.png)

### 

### Save Well Case and Run

* Perform File -&gt; Save Well Case Click 
* Run Simulation button

![](.gitbook/assets/image.png)



### Get Started with Netool Simulation Results

* Inspect Results 
* Look at Summary Table 
* Look at the plots and customize 
* Analyse Detailed Plots of different parameters to understand performance

![](.gitbook/assets/image%20%2830%29.png)







## Well target, IPR and Well Performance Curve

