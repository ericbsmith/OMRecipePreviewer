# OMRecipePreviewer
Bulk generate JPEG renders of OM Recipes using OM Workspace on macOS using Applescript
Can be run using Shortcuts or Automator

## OM Workspace
Photo editing software from OM System for users of OM System/Olympus digital cameras

## OM Recipes
Creative recipies which can be used in OM System OM-3 cameras but can also be applied to OM System/Olympus RAW files via OM Workspace. 

Useful recipe sources: 
- https://om-recipes.com/
- https://explore.omsystem.com/us/en/creative-recipes

## Prerequisites
1. Enable control of OM Workspace on your machine (System Settings/Privacy & Shortcuts/Accessibility... enable Shortcuts and/or Automator)
   <img width="724" height="309" alt="Enable control" src="https://github.com/user-attachments/assets/f63c1c55-5534-4375-9296-82c86186a81f" />

2. Create a folder called "OMRecipePreviewer" within your user home
3. Create a sub-folder called "recipies"
4. Add an Olympus RAW file as "sample.ORF"
   <img width="583" height="118" alt="Folder Structure" src="https://github.com/user-attachments/assets/23b34fdf-60c8-4c97-b769-7a885ddf908e" />

5. Download/copy all recipes you wish to apply to the "recipes" folder. **Filenames must not contain spaces.**

## Create a new Shortcuts or Automater task
The script can be run via Shortcuts or Automater. Create a new task in your chosen method.

### Shortcuts
Add a Run Applescript step
   <img width="835" height="239" alt="Shortcuts Screenshot" src="https://github.com/user-attachments/assets/5cacc259-b2a0-463a-b3f9-d863452f89a5" />

Replace the text (* Your script goes here *) with the contents of the [applescript.txt file](applescript.txt)

### Automater
Add a Run Applescript step to a Workflow document
   <img width="529" height="244" alt="Automater Screenshot" src="https://github.com/user-attachments/assets/bb3509ae-1e4d-434a-b250-18e035bb806f" />

Replace the text (* Your script goes here *) with the contents of the [applescript.txt file](applescript.txt)





