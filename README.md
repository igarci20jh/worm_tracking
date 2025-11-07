## Worm Tracking Code (initial-code-11-07-2025.ipynb)
To Run this code you must change the following:
- **PathName** to the path folder the frames are stored in (this is in the first code block)
- **numberOfWorms** to the number of worms seen in the cropped video (this is in the second code block)
- **pixels_per_mm** this is a conversion factor to change this you can make a line in image j spanning from one side of the plate to the other. Take the number of pixels that line is and divde by 150mm (since the plate is 15cm).
- **frames_per_minute** if frame rate changes

**Notes:**
- If you are using the ringlight to record the videos you may have to invert the video in fiji first because we had issues which the code not being able to read the frames otherwise. (not sure how to fix this yet)

- The code block that calculates reorientations of the worms definitely needs work especially the code block to calculate all the reorientation rates from all the worms in the video. We must add a limit to change in theta that the code will consider a reorientation (60 degrees or about 1.04 radians). We must also wrap to pi. 

## Optimizing Video Taking Spreadsheet
This Excel sheet has the different setting used to take a total of 11 videos and how well the code tracked the worms in the video based on the worms tracked, frames dropped, and number of worms tracked through the whole video. The best camera settings are the row that is colored grey. The last three rows are three videos recorded with these optimal settings using the worm tracking code. There are NAs in the distance column because this was no longer needed after the settings were optimized. There are notes in some of the cells that describe what certain columns are in case it is difficult to understand.

## Rotation Talk Powerpoint
Gifs for this powerpoint were taken from the 101425-inverted folder on the F drive of the microscopy computer. This is the video we took with the ringlight but inverted using fiji. Only certain frames were shown and the code for the graphs are in the code blocks named "Reorientation graphs for worms 3 & 5 in specific frames" and "velocity graph for 2 specific worms in specific frames".

## Data Storage
Videos taken during this rotation are saved in the DATADRIVE3(F:) on the microscopy computer in a folder named "IsabelG".
