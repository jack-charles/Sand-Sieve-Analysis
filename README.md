# Sand-Sieve-Analysis

This is a script to interpret results from a sand sieve test, calculating the cumulative weight percentages, various size and sorting factors, and allow plotting of results with selected screens and proppants.

For a quick demo mode, enter 100 at the menu to read the default data and provide graphs.

Description of options and recommended order

1 - Open sieve data file. This will be a typical sand sieve analysis file of weight retained per mesh size. File format is Name of sample, Depth, and weight retained on a mesh size. Mesh sizes must be the same for all entries per uploaded files, however upon assignment the mesh sizes will be stored for each sample.

2 - Open saved file. The program will ultimately create a JSON file that will save the sand sieve data and all calculations performed with it. Each entry will have it's own set of mesh sizes with it, so this JSON can accommodate samples that were done with different meshes, say if you had old data from a different sieve shaker that you wanted to compare new results with.

3 - Append new sand sieve data. This allows for multiple sand sieve analysis files to be merged together. The new file is opened as usual, assigned to a list, and then merged with an existing dataset. Note this will still work if the existing dataset is empty.

4 - Import screen data. Import screen name, type, and aperture (slot width or pore size), and assigns to a dictionary.

5 - Import proppant data. Imports proppant name, permeability, specific gravity, absolute volume, bulk density, and D50, and assigns to a dictionary. This data is usually provided by the manufacturer. For best results, use permeability that is based on the confining stresses that will be observed.

6 - Select screen. Select which screens you want to plot with. You must select this for each screen you want to add.

7 - Select proppant. Select which proppants you want to plot with. You must select this for each proppant you want to add.

8 - Select units. Select which unit the sand sand sieve data is imported with. This script will use microns internally and for display.

10 - Perform calculations. Determines the cumulative weight percentages and other factors.

11 - Print SRT data. Outputs in the terminal the data calculated for all samples.

12 - Plot results. Plots a series of useful graphs for analyzying the sand samples, and plots screen and proppant sizes to help determine which is suitable.

20 - Save file. Saves all information, including calculations and selected screens and proppants, to a JSON file.

0 - Quit. Quits program.
