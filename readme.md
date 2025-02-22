Create virtual environment
mkdir proj_dir
cd proj_dir
python3 -m venv .venv
#activate
source .venv/bin/activate

/*
deactivate
*/

#Create a base file with required libraries in requriements/requirements.in
#run the following to create requriements.txt
pip-compile-multi

#install requriements
pip install -r requirements/requriements.txt

#Initialize git from this folder

