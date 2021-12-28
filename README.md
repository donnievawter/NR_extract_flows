# NR_extract_flows
This a simple node-red flow that extracts the info for each tab and creates a json file for it.
It does the same thing you can do manually using the export menu but extracts for all the flows.
You will have to enter the full path to your flows.json file and the full path to the directory where you want to save the files.
The file names are the names of the tabs with any spaces replaced with an _ e.g. Flow_1
The JSON file created is an array of objects, the first being the tab and subsequent being the nodes on the tabs.
