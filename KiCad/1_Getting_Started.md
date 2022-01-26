# Getting Started with KiCad

KiCad is our PCB design and layout software. We'll have a project folder here to test your KiCad install. Follow the directions to get everything setup and create your first project. 

Assumptions: You read and understand the GitHub tutorials and know how to clone, pull, and push files. If that doesn't sound familiar, stop and go look at those tutorials now. 

Now, let's get into installing the application and setting up the project files.

## Setting up the Application Environment

You'll need to install [KiCad Version 6.0](https://www.kicad.org/download/). There was a major update in the file system that changes the libraries and schematic systems. We are designing using version 6.0, so if you've installed KiCad earlier (i.e. V5.1) you'll have to uninstall and reinstall the application.

### Linking Libraries

If you have a fresh install of KiCad, you shouldn't have any library issues. If you had to reinstall the new version, libraries can be tricky due to different versions. Either way, you'll need to link the AERO custom libraries. To do this, open KiCad and go to `Preferences` -> `Manage Custom Symbols` and `Manage Custom Libraries`. 

You'll need to clone the `AERO_KiCAD_Library` repo. The symbols are all in the `AERO_custom_symbols.lib`. The footprints are in the `CustomFootprints.pretty`. When adding these libraries to the kicad preferences, you'll need to call the symbols `AERO_Symbols` and the footprints `AERO_Footprints`. These names are very important as they are referenced across libraries.

## Beginning your first project

There are a few video tutorials to get you started using kicad. This covers how to setup a schematic, pick components and layout a board. The videos are in the AERO teams general channel with links below. If you have any trouble accessing these videos please let an AERO member know. Note, these videos were done in KiCad Version 5.1, so some of the icons changed, but the general information is the same.

 - [Setting up KiCad](https://web.microsoftstream.com/video/3cbb63a3-6bf1-4e11-8af3-7573031418f2) (be sure to read [Linking Libraries](#linking-libraries) for naming convention first!)
 - [Creating a Schematic](https://web.microsoftstream.com/video/889c0a42-7ca3-48a4-8e2d-93239870cec9)
 - [Board Layout](https://web.microsoftstream.com/video/b89a2ec7-5980-4a40-be36-78aff48dd095)
 - [Plotting Gerber Files](https://web.microsoftstream.com/video/cbaff215-120e-4109-a0d7-6708654a2546)

 ## Next Step

 Alright, now let's do one with version control (Git). [Continue to step 2](2_Modifying_KiCad_Files.md)