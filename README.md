# Assignment 2 Stolen Model Detection.
The folder contains the code and the steps to achieve the best score in assignment 2 - Stolen Model Detection.

## Files
- README.md - explains how to recreate the best result
- ensemble_v49.py - Contains the script
- submission.csv - contains the final submission file generated
- features_v21_perm_invariant.csv - feature file (set) used by the ensemble script
- detect_perm_invariant_v21.py - generates the feature file


How to Setup and Run:

1. create working directory using `mkdir -p ~/tml26_task2_work` in cluster.
2. Then download files provided from the repository.
3. Go to the directory, create and activate python virtual environment, using
   `python3 -m venv .venv`
   `source .venv/bin/activate`
4. Install dependencies,
   `pip install --upgrade pip`
   `pip install torch torchvision pandas numpy safetensors tqdm`
5. The feature file `features_v21_perm_invariant.csv`is already included.
6. Therefore, run the script, `python ensemble_v49.py`.
7. This creates the final submission csv file.
8. To use it as the official submission file, `cp submission_v49.csv submission.csv`.
9. Then Run, `python submission.py`.

Regenrating the feature file :

1. The feature file can be regenrated with, `python detect_perm_invariant_v21.py`.
2. Make sure the provided files are present, official/target_model/weights.safetensors and http://official/suspect_models/.
3. Once feature file is generated, run the script using `python ensemble_v49.py` (follow step 6 onwards)
