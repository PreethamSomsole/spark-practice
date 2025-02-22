# Create virtual environment
mkdir proj_dir \
cd proj_dir \
python3 -m venv .venv \
#activate 
source .venv/bin/activate \

/*
deactivate
*/

# Create a base file with required libraries in requriements/requirements.in
# run the following to create requriements.txt
pip-compile-multi

# install requriements
pip install -r requirements/requriements.txt

# https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github
# Initialize git from this folder
git init -b main
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

$ git add .

# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use  # 'git reset --soft HEAD~1' and commit and add the file again.

$ git commit -m "First commit"

git remote add origin https://github.com/PreethamSomsole/spark-practice.git
git branch -M main
git push -u origin main

