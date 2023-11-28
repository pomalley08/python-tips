# New Project Setup
Here's the steps I take frequently to setup a new python repo for future reference.

## Create new venv
1. Use the specific python version to make a new venv for the repo  
`cd new-repo`  
`path/to/python -m venv {env name}`
2. Activate the new venv  
windows: `.\{env name}\Scripts\Activate.ps1`  
macos/linux: `source {env name}/bin/activate`
3. Install packages

## Create ipykernel kernel based on the venv
Enables use of the packages in the venv in jupyter notebooks
1. Install ipykernel in the venv  
`pip install ipykernel`  
2. Create the new kernel  
`python -m ipykernel install --user --name {env name}`
