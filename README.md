# NMS-Creature-Builder
--------------------------------------------------------------------------------------------
NMS Creature Builder - Created by laanp
--------------------------------------------------------------------------------------------
This Excel workbook was created to facilitate management & modification of No Man's Sky pet
information.

The workbook allows import/export of pet information text via the Windows clipboard to/from 
the No Man's Sky Save Game Editor, (by GoatFungus - https://github.com/goatfungus/NMSSaveEditor) 

The workbook configuration form, allows modification of key pet features, including:
	- Creature ID  - (ie; what type of pet)
	- Size
	- Physical attributes (ie; heads, body & tail types, horns eyes, ears scales etc)
	- Pet Name
	- Seeds (ie; primary/secondary colors, textures, bone shape, species and genus) 
	- Fur (flag to set if animal can have fur - not applicable to allpets)
	- Age - (not fully implemented yet)
	- Home Biome (where they are from and where you can induce an egg)
	- Unique ID - This needs to be randomized to ensure your created pet is visible to 
		      other players, the way you made it.
	- Trust, Traits and Mood adjustment sliders (how aggressive, playful or devoted your pet is)

The tool also allows you to save & load preset pet configurations (*.txt) files, that can be opened,
modified and exported to the Windows clipboard, for import into the game save file using the
No Man's Sky Save Game Editor.

--------------------------------------------------------------------------------------------
Youtube: [How To Use This Tool](https://youtu.be/imNyf0Twseg?si=1q4KYMkeIb0O9D_t) 

GitHub Download: [NMS Creature Builder - Latest Release](https://github.com/laanp/NMS-Creature-Builder/releases/tag/v1.6)


--------------------------------------------------------------------------------------------
Requirements:
--------------------------------------------------------------------------------------------
This is a macro-enabled Microsoft Excel workbook, (.xlsm) and you will need a copy of the 
latest version of Microsft Excel 365 Office to use it.

You will need:	- Microsoft Excel - Office 365 (might work on earlier versions of Excel, but has not been tested)
		- No Man's Sky Save Game Editor (v1.10.7 or later), (by GoatFungus - https://github.com/goatfungus/NMSSaveEditor) 
		- Your favourite photo editor, that can handle *.jpg files 
		     (the editor is needed to view/save your pet screenshots)   		


--------------------------------------------------------------------------------------------
Installation:
--------------------------------------------------------------------------------------------
Download the latest version from GitHub (see above URL): 

Unzip the contents of the "NMS Creature Builder vx.x.zip" to any folder on your hard drive
There are several sub folders in the zip file, and they are fixed:
		\EXML\		- contains the extracted *.EXML creature information files (column L in the Data sheet)
		\Templates\  	- contains specific customized pet text & jpg files 
		\Pics\		- contains generic pet images (no seed info, just shows what the creature attributes are)


Run the "NMS Creature Builder (vx.y).xlsm" in Microsoft Excel, the workbook is not protected, so if you are interested in 
looking at the VB code behind the tool, feel free to dive in.

The EXML files included in this installation package, will be current from the No Man's Sky version compatibility noted
at the top of this file.

The pet information files are formatted as matching *.txt & *.jpg files and are in the following format:
<creatureID>_xxxxxx'xxx-<pet name>.txt

The <creatureID> will be the main pet creature ID - a complete list is in column L on the Data sheet
the xxx'xxx are the specific attributes of the pet from 1-18, with the apostrophe indicating the next position of a 2 digit 
attribute.   for example:
	CAT_111118111'14-My New Pet.txt

Will be the CAT creatureID, with (10) attributes, all attribute dropdowns will be set to the 1st dropdown selection except 
the 6th attibute, which is set to 8th dropdown selection, and the 10th attribute, which is set to the 14th dropdown selection. 

And finally, the last part is the name of the pet, as I decided to add this into the file naming convention to allow 
saving of multiple pets, that perhaps have the same physical attributes, but might be different colors.  Pet names should
be used that are unique to facilitate this file management scheme.


--------------------------------------------------------------------------------------------
Example on How To Use The Program
--------------------------------------------------------------------------------------------
The workflow goes something like this:

1. While in-game, you might come across a unique creature you want to save or modify.  Make the creature your pet in the
   usual way, and take a screenshot either in the "Creature"..."Companion Register" menu in-game, or using photo mode
   while it's running around.

2. Jump into/out of your ship to save your current game, and go into the No Man's Sky Save Game Editor, load up your save,
   and copy the particular pet info to the Windows clipboard. 

3. Load up the NMS Creature Builder Excel file, click on the Config Form button to bring up the form.  Click the "Import"
   button on the form to load up the pet info currently in the clipboard, onto the form.

4. Make sure you select the "Keep Seeds" & "Process Image" checkboxes beside the Save button.  Click on the save button and it will automatically 
   bring up the proper text file to save your seeds and pet info into the library.

5. After save the template text file, the program will launch your favourite pic editor and load the name of the latest 
   screenshot file (located in the \Screenshots\ folder - also controlled by the "settings" button) in the picture 
   viewer/editor (program associated with *.jpg files)

5. Resize the picture (to save on file storage, I usually size them to 800x600) and when you go to save it... hit the CTRL + V to paste the correct name into the 
   Saves ... as... filename box of your favourite picture editor, from the Windows clipboard (this full filename
   is generated automatically in code and copied to the clipboard when you click the save button)

6. Now you have the *.txt file and the *.jpg library files saved. You can pull these files into the config form any time
   by clicking the Load button and selecting the appropriate text file.  Try changing some attributes, click the "Update
   Pet File" button, and then the "Export" button, and paste the Windows clipboard contents into the save game editor, and
   save the changes. 
   
7. Reload the game on the last updated save file and enjoy your new pet! 

I am also working on some video tutorials on how to use the program, which will be accessible on my YouTube channel (see below):


Enjoy!

[Peter Laan - NMS YouTube Channel](https://www.youtube.com/c/PeterLaan)

