# SE Robotics School
This is the repository for the website of the "Summer School for Software Engineering in Robotics" series.

## Building the SE-Robotics Summer School webpages
To build the webpages locally, the environment needs to be setup by running the following (assuming the repo is already cloned).
```sh
cd docs/
python3 -m venv venv
source venv/bin/activate # (Or your OS specific equivalent)
pip install -r requirements.txt
```

Afterwards to build the pages run the following from the docs folder:
```sh
# Make sure the Python environment is sourced
# Linux: source venv/bin/activate

# For a normal build
sphinx-build source build

# For a build which, updates the TOC/Navigation sidebar
sphinx-build source build -Ea
```
