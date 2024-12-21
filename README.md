```bash
echo '\nDeactivating all active conda environments\n\n'
conda deactivate 2>/dev/null || true
echo '\nRemoving "neural_network" environment\n\n'
conda remove --name neural_network --all -y
echo '\nRecreate "neural_network" environment\n\n'
conda env create -f environment.yml -y
echo '\nActivate "neural_network" environment\n\n'
conda activate neural_network
```

# neural-network-challenge-1
How likely are YOU to pay your loan on time?


# Getting Started
- Download starter files from module challenge
- read CSV from:  https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csv

# Part 1: Prepare the data
- Use scikit-learn StandardScaler()
- X = features
- Y = Targets (credit_ranking)

# Part 2: Compile and Evaluate Models
 - TensorFlow (binary_crossentropy, adam optimizer, and accuracy)
 - Save and export results with student_loans.keras