# Yeast Tranformation Protocol
Automated yeast transformation using lithium acetate for Opentrons 2.
1) Automated pipetting of transformation mixture and yeast cells
2) User will move plate onto temperature module
3) Opentrons heat shock cells and transfers the samples to a new sterile plate
4) User will centrifuge plate and return to Opentrons robot
5) Automated resuspension of cells in calcium chloride
6) Plate is now ready for incubation and plating

Download the folder from GitHub
-------------------

![Save GitHub folder on to your computer](https://i.postimg.cc/1t8HdhjY/Screenshot-2020-12-14-at-15-56-09.png)



Creating your customised protocol
-------------------

Open terminal or command line and change the directory (‘cd’):

	$ cd YourFilePath/Yeast_Transformation_OT-main/Opentrons_scripts 
 
Run the script using python by typing the following:

	$ python YeastTransformationProtocol_API2.py
	

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

Please set up your Opentrons as shown in the image above. 

The reervoir should contain:
- A2 --> Lithium acetate and single stranded DNA
- A4 --> PEG
- A6 --> Calcium chloride
- A8 --> Yeast cells at appropriate OD
- A9 --> Water
- A12 --> Waste well
