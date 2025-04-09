Vesicle Tracking GUI for Multi-Frame TIFF Images
This MATLAB script implements a graphical user interface (GUI) for tracking vesicles in multi-frame TIFF images. The application enables users to load TIFF files, select regions of interest (ROIs), and process multiple frames to measure the intensity of vesicles over time. 

Features
Load TIFF Files: Users can select and load multi-frame TIFF files.
Select ROI: Allows users to draw a polygon around vesicles in the first frame.
Process Frames: Processes each frame to calculate the maximum intensity of vesicles over time. The results are displayed in a plot that illustrates intensity changes across frames.
Save Results: The intensity plot is automatically saved as a PNG file.
GUI Components
Load TIFF Button: Opens a file dialog to select TIFF files.
Select ROI Button: Allows users to draw a polygonal region around the area of interest in the displayed image.
Process Button: Begins processing the images to analyze vesicle intensities.
Usage
Run the Function: Call the vesicleTrackingGUI_TIFF() function in the MATLAB command window.
Load a TIFF File: Click on the "Load TIFF" button and select a multi-frame TIFF image.
Select a Region of Interest: Click on the "Select ROI" button and draw a polygon around the vesicle region in the first frame.
Process the Images: Click on the "Process" button to analyze the frames. The GUI will display the current frame being processed, and after processing, a plot of vesicle intensity over time will appear.
View the Results: The resulting intensity plot is saved as vesicle_intensity_tiff_plot.png in the current directory.
Technical Details
Data Structure: The script uses a 3D array to store the image stack, with dimensions corresponding to height, width, and frame number.
Image Processing: It employs thresholding and binary image processing techniques (using imbinarize and regionprops) to isolate vesicle regions and calculate their intensities.
Dependencies: Requires MATLAB's Image Processing Toolbox.
To use the GUI, simply execute: vesicleTrackingGUI_TIFF();
After loading a TIFF file, select the ROI and process the frames as instructed.
MIT License

Copyright (c) [2025] [Muralidharan Mani]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
