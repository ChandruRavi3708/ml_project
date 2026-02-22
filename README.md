# ML Project – Git & GitHub Version Control Assignment

This project demonstrates the use of Git and GitHub for version control in a Python machine learning workflow.

## Project Structure

The project contains the following files:

- train.py – Model training script
- predict.py – Prediction script
- utils.py – Helper functions
- config.py – Configuration settings (added during collaboration stage)
- README.md – Project documentation

---

# Stage 1: Basic Setup (Foundation)

The following commands were used to set up the project:

```bash
cd ~
mkdir ml-project
cd ml-project
git init
touch train.py predict.py utils.py README.md
git status

# Stage 2: Version Control Workflow (Application)

After adding code to train.py and utils.py, the following commands were used:

git add train.py utils.py
git commit -m "Add training script and utilities"
git branch -M main
git remote add origin https://github.com/ChandruRavi3708/ml_project.git
git push -u origin main


Stage 3: Collaborative Workflow (Synthesis)

Scenario:

Teammate updated predict.py and README.md on GitHub.

Locally modified utils.py and created config.py.

Step 1: Check Status
git status

To see modified and untracked files.

Step 2: Stage and Commit Local Changes
git add utils.py config.py
git commit -m "Update utils and add config file"

This ensures local work is saved before pulling updates.

Step 3: Pull Remote Changes
git pull origin main

Fetches and merges teammate’s changes.

Step 4: Push Final Version
git push origin main
