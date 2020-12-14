# Yeast Transformation Protocol

Reagents (volumes for transforming one sample):
- 1M Lithium acetate (18 µl)
- 10mg/ml Salmon sperm DNA (5 µl)
- 50% PEG-3350 (120 µl)
- DNA mini-prep
- Yeast cells at appropriate OD (32 µl)
- 5mM Calcium chloride (200 µl)

Opentrons equipment:
- 2x 96 well plates
- 2x temperature modules (GEN 2)
- 4x 24 eppendorf rack
- 12 well reservoir
- p300 multi pipette (GEN 2)
- 2x 300 µl tiprack
- p20 single pipette (GEN 2)
- 20 µl tiprack

Download the folder from GitHub
-------------------

![Save GitHub folder on to your computer](https://i.postimg.cc/1t8HdhjY/Screenshot-2020-12-14-at-15-56-09.png)



Creating your customised protocol
-------------------

Open terminal or command line and change the directory (‘cd’):

	$ cd YourFilePath/Yeast_Transformation_OT-main/Opentrons_scripts 
 
Run the script using python by typing the following:

	$ python YeastTransformationProtocol_AP12.py
	

Prompts will appear, as shown below. Enter the specific values for your experiment.

![Save GitHub folder on to your computer](https://i.postimg.cc/cLFZ72tb/Screenshot-2020-12-14-at-16-23-20.png)

Ignore the following errors (They appear because the computer is not connected to an Opentrons):
  
	$ /.opentrons/deck_calibration.json not found. Loading defaults
	$ /.opentrons/robot_settings.json not found. Loading defaults


Enter new file name. 

The new file will be saved in the Opentrons_scripts folder.

You can now run this in the Opentrons app!

Creating a separate file for your experiment helps to protect the original script from user-specific changes. 

Further help
-------------------

Follow the link to watch a detailed demonstration of how to download and implement this code.

https://www.youtube.com/watch?v=-7qC8O_KkY4&fbclid=IwAR1L49QSFspqv5ncrnHhUJSvyippbG5xk71tXlP7UXx7C4ILsos51kv6wh0

Opentrons set up
-------------------

![Save GitHub folder on to your computer](https://i.postimg.cc/pdj3q73J/pasted-image-0.png)

Please set up your Opentrons as shown in the image above. Place a 96 well plate onto the cold block.

The reservoir wells should contain:
- A2 &#8594; Lithium acetate (1.8 ml) and salmon sperm DNA (475 µl)
- A4 &#8594; PEG (11.5 ml)
- A6 &#8594; Calcium chloride (19.5 ml)
- A8 &#8594; Yeast cells at appropriate OD (3.2 ml)
- A9 &#8594; Water (20 ml)
- A12 &#8594; Waste well

(Can adjust volumes for number of samples you are transforming)

Automated protocol
-------------------

1) Adds lithium acetate (18 µl) and salmon sperm DNA (5 µl) to all wells of 96 well plate on cold block
2) 120 µl PEG is added to all wells 
3) DNA mini-preps will be added to specific wells
4) 32 µl yeast cells are added and mixed thoroughly
5) User must move 96 well plate onto hot block 
6) Cells undergo heat shock
7) Opentron transfers cells to clean 96 well plate 
8) User centrifuges plate and returns to deck
9) Supernatant is removed
10) Cells are mixed with 200 µl calcium chloride
11) Plate can be removed for incubation and plating


