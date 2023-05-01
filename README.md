# Process Mining & Machine Learning to predict medical diagnoses codes
This repository contains the python notebook and usage instructions for my Bachelor's Computer Science project titled above. The supervised learning models built were used to evaluate whether a combined process mining and machine learning approach can be used to enhance the clinical coding process within healthcare.

# Usage
Guidelines to run the notebook in two ways are given below

## End-to-end (required for first run):-
1. Run the cell under ‘Authentication & Connecting to MIMIC-III’
   1. Requires access to the MIMIC-III dataset on BigQuery via the users google account. Change the client number in the cell accordingly
   2. Comment out the mounting of google drive
2. __SKIP__ the cell under ‘Load Dataframes from Google Drive’
3. Run all cells under ‘Event Log Creation’
4. Run all cells under ‘Combining Event Logs’
5. Run the cell under ‘Calculate duration for each trace’
6. Run all cells under ‘Prepare Feature Data’
7. Run all cells under ‘Prepare Target Data’
8. Run all cells under ‘Train-Test Split & Apply Pre-processing Pipeline’
9. Cells under ‘Find best algorithms’ __NEEDN'T__ be run because they take a long time (especially the 2nd cell)
10. Under ‘Train & Test models’
    1. The first 4 cells __NEEDN'T__ be run because they take a long time
    2. Run all remaining cells
11. _Optionally_, run the cell under ‘Saving Dataframes to Google Drive’. This will streamline future notebook runs by allowing the user to load dataframes from their google drive (if no changes need to be made to the event log and feature data)


## Loading dataframes from Google Drive:-
1. Run the cell under ‘Authentication & Connecting to MIMIC-III’
   1. Requires access to MIMIC-III on BigQuery via the users google account. Change the client number in the cell accordingly
   2. Requires dataframes to be available on users google drive from a previous run
2. Run the cell under ‘Load Dataframes from Google Drive’
3. __SKIP__ all cells up to ‘Train-Test Split & Apply Pre-processing Pipeline’
4. Follow end-to-end usage notes from (and including) step 8, till the end
