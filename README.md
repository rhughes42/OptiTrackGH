# Tracker
A Grasshopper plugin for NaturalPoint's NatNet API. Supports real-time motion tracking with OptiTrack camera systems. 

Requires a valid copy of the OptiTrack Motive software to broadcast MoCap data on a local network.
Tracker grabs frame data from Motive, scales, translates and presents the relevant Rhino Geometry inside Grasshopper. Using basic interaction, this can be used for tracking tools, calibrating and tracking robotics applications, structural materials testing and much more.

Read more about OptiTrack here: https://optitrack.com/applications/

## Dependencies
Tracker requires version 4.0 the NatNet Assembly (NatNetML.dll), which is included in this repo in the lib folder.  
The full SDK can be downloaded from https://optitrack.com/software/natnet-sdk/

## Installation
1. Right-click the Tracker.zip file, go to 'Properties' and check 'Unblock' if present, then 'Apply / OK'.
2. Unzip the file to your Grasshopper libraries folder.  
3. Restart all running instances of Rhino.

## Usage
The plugin now only contains one real component for catching broadcasted frames from a running instance of Motive.  

You will need a valid OptiTrack setup and a license for motive before anything will appear on your local network.  

This plugin will catch them, do some optimization to make sure we don't redraw every single frame (this can be turned off), and then creates some Grasshopper geometry to represent the position of the Motive frame. It has application in architectural robotics, production, game design, motion capture etc.

### Contributors
Ryan Hughes  
Povl-Sonne Frederiksen
