# Make-o-Matic
## Gesture Recognition with Machine Learning

a project by TU Wien and Laber's Lab

contributors: Thomas Lidy

## Installation

Python 2.7 is required.

We have tested on Ubuntu 16.04.3 LTS.

Clone this repository.

All required Python models are installed by this:

pip install -r requirements.txt

All code is provided and run inside iPython / JuPyter notebooks, which also needs to be installed.


## Data

The sub-folder ''data'' contains all metadata json files, but not the actual data export from the database.

The data export we used is called ''EXPORT_09042017173622.csv'' and needs also to be placed in the data sub-folder.

## Execution

The program is split into 3 parts:

1. data-preparation.ipynb
2. testing.ipynb
3. machine_learning.ipynb

### Explanation:

1. data-preparation.ipynb

Is the pre-processing of the data, data cleansing and removal of unneeded data.
The prepared data will then be exported to a new csv file in the data sub-folder, which is needed by steps 2 and 3 as an input.

2. testing.ipynb

Here, important processing steps such as Time normalization, resampling, min-max normalization, processing and isolation of individual
gestures, etc. are tested, experimented with and visualized so that their impact can be understood.

3. machine_learning.ipynb

Here, the essential parts of testing.ipynb are repeated, and implemented in a compact way. No visualization or extra steps are used here.
This means a fast processing for the machine learning and a fast feature extraction.
Feature extraction is the step of extracting semantically meaningful derived data from the input which serves as the basis for Machine Learning.
Ultimately, a range of Machine Learning experiments are started here, with results presented in nice HTML tables.

NOTE: Step 1 needs to be executed only once, and step 2 is for information purposes only.
So step 2 can be skipped and you may immediately proceed to step 3, where the output of step 1 is read in, and the Machine Learning
processes are started.