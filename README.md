# Assignment2 
The repository contains the script for best score in assignment 2.

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
5. First generate the feature file using, python src/detect_perm_invariant_v21.py. This creates features_v21_perm_invariant.csv
6. Then run the ensemble script, `python src/ensemble_v49.py`.
7. This creates the final submission csv file.
8. The make it as the official submission script.
9. Then Run, `python submission.py`.
