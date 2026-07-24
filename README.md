sudo apt install python3.10-pip      # for ubuntu

python -m pip install --upgrade pip   # for win

==================================================================

sudo apt install python3.10-venv   # for ubuntu

python -m venv myenv  # Replace "myenv" with your environment name   for win & linux

.\myenv\Scripts\activate   # win cmd powershell

source myenv/bin/activate  #linux

source onmsioss/Scripts/activate  ##git bash


pip list 

pip install -r requirements.txt

pip list

pip show <package_name> 

#allows you to select the environment in Jupyter Notebook
pip install ipykernel

#Add the virtual environment to Jupyter
python -m ipykernel install --user --name=onmsioss


=========================================================================
import sys                                                              =
print(sys.executable)  # Should point to your venv Python               =
=========================================================================


#Deactivate the environment
deactivate

#Remove the kernel
jupyter kernelspec uninstall <myenv>

##### by using CLI

jupyter nbconvert --to html <your_notebook.ipynb>

jupyter nbconvert --to html --no-prompt <your_notebook.ipynb>

jupyter nbconvert --to script <your_notebook.ipynb>

jupyter nbconvert --to script --no-prompt <your_notebook.ipynb>

##### by using cell in markdown  Inside a Jupyter Notebook (Programmatic)

!jupyter nbconvert --to html <your_notebook.ipynb>

!jupyter nbconvert --to html --no-prompt <your_notebook.ipynb>

!jupyter nbconvert --to script <your_notebook.ipynb>

!jupyter nbconvert --to script --no-prompt <your_notebook.ipynb>


====================================================================================

###  Git & GitHub

sudo apt update                         # update os package

sudo apt install git -y                 # Installing Git

git --version                           # for verification

----------------------------------------------------------------------------

git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"


-------------------------------------------------------------------------

Scenario A: Uploading a Local Project to GitHub
If you have an existing directory of code on your Ubuntu machine that you want to send to GitHub:
Initialize the local folder as a tracking repository:
    bash
        cd /path/to/your/project/folder
        git init

Stage your files to prepare them for recording:
    bash
        git add .
Commit the files with a descriptive snapshot message: 
    bash
        git commit -m "Initial project commit"


Connect and push your local branch directly to that online folder:
    bash
        git remote add origin git@github.com:username/repo.git
        git branch -M main
        git push -u origin main


git remote set-url origin https://github.com/monem-ali/testing.git

git config --global credential.helper store

git push -u origin main

git remote add origin https://github.com/monem-ali/testing.git
git branch -M main
git push -u origin main

========================================================================



