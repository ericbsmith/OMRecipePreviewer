# OMRecipePreviewer
Bulk generate JPEG renders of OM Recipes via OM Workspace on macOS using Applescript in the [Shortcuts](https://support.apple.com/en-gb/guide/shortcuts-mac/apdf22b0444c/mac) or [Automator](https://support.apple.com/en-gb/guide/automator/welcome/mac) programs

## OM Workspace
Photo editing software from OM System for users of OM System/Olympus digital cameras

## OM Recipes
Creative recipies which can be used directly in OM System OM-3 cameras but can also be applied to any OM System/Olympus RAW file via OM Workspace. 

Useful recipe sources: 
- https://om-recipes.com/
- https://explore.omsystem.com/us/en/creative-recipes

## Prerequisites
1. Enable control of OM Workspace on your machine (System Settings/Privacy & Shortcuts/Accessibility... enable Shortcuts and/or Automator)
   <img width="724" height="309" alt="Enable control" src="https://github.com/user-attachments/assets/f63c1c55-5534-4375-9296-82c86186a81f" />

2. Create a folder called "OMRecipePreviewer" within your user home folder
3. Create a sub-folder called "recipes"
4. Add an Olympus RAW file an rename as "sample.ORF"
   <img width="583" height="118" alt="Folder Structure" src="https://github.com/user-attachments/assets/23b34fdf-60c8-4c97-b769-7a885ddf908e" />

5. Download/copy all recipes you wish to apply to the "recipes" folder. **Filenames must not contain spaces.**

## Create a new Shortcuts or Automater task
The script can be run via Shortcuts or Automater. Create a new task in your chosen method.

### Shortcuts
Add a Run Applescript step
   <img width="835" height="239" alt="Shortcuts Screenshot" src="https://github.com/user-attachments/assets/5cacc259-b2a0-463a-b3f9-d863452f89a5" />

Replace the text (* Your script goes here *) *including the brackets* with the contents of the [applescript.txt file](applescript.txt)

### Automater
Add a Run Applescript step to a Workflow document
   <img width="529" height="244" alt="Automater Screenshot" src="https://github.com/user-attachments/assets/bb3509ae-1e4d-434a-b250-18e035bb806f" />

Replace the text (* Your script goes here *) *including the brackets* with the contents of the [applescript.txt file](applescript.txt)

## Generating JPEGs
To generate a JPEG for each recipe:
1. Exit OM Workspace if it is currently open
2. Run your Shortcut/Automater job
3. Wait for the automation to cycle through the process
4. Make a coffee (depending on how may recipes are being applied)
5. JPEGs are created in the "OMRecipePreviewer" folder and are named with the recipe filename. This allows you to identify any recipes which you prefer. They will also be visible in OM Workspace at the end of the process

## Known issues
1. Currently Keystone Compensation causes the process to error - due to the pop-up in OM Workspace informing that it may not be applied correctly. Workaround: remove any Keystone Compensation step in the offending .OES file
2. Wait times in the script are guesstimates based on an M4 MacBook Pro. You may need to increase these if you encounter any issues

## Regenerating Tips
- Either delete all previously generated JPEGs or move to another folder to avoid numberic copies of files being generated on the next run
- Perform the Generating JPEGs steps above

## Adding new recipes
Simple add the .OES file to the "recipes" folder and regenerate




