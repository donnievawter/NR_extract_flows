# NR_extract_flows
This a simple node-red flow that extracts the info for each tab and creates a json file for it.
It does the same thing you can do manually using the export menu but extracts for all the flows.
You will have to enter the full path to your flows.json file and the full path to the directory where you want to save the files.
The file names are the names of the tabs with any spaces replaced with an _ e.g. Flow_1
The JSON file created is an array of objects, the first being the tab and subsequent being the nodes on the tabs.

# Usage
1. import Generate_Flow_Files.json into node-red
1. change the path in the read file node to point to your flows.json
1. change the path inthe function to point to the directory where the results are stored
1. Deploy
1. Click on the inject node to generate the files:
2. If you want to back up files after every deploy change the inject node to fix x seconds after startup instead of triggering manually. git is smart enough to realize the files are unchanged even if you overwrite so only flows that actually change will need to be committed.
WARNING: Each time you run this it will overwrite any earlier generated files.

