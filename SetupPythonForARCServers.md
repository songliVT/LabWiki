### This page contains some instructions for setting up Python for ARC servers at Virginia Tech.

ARC default python does not include pip and virtualenv. This instruction assume the working directory is ````$HOME````

#### Step 1. install PIP in a user directory
Instruction for install PIP can be found here: https://packaging.python.org/installing/

````
cd $HOME
mkdir .local
mkdir download
cd $HOME/download
wget https://bootstrap.pypa.io/get-pip.py
python get-pip.py --prefix=$HOME/.local
````

#### Step 2. add PIP in PYTHONPATH
````
vi ~/.bashrc
# add two lines to .bashrc
## export PATH=$HOME/bin:$HOME/.local/bin:$PATH
## export PYTHONPATH=$HOME/.local/lib/python2.7/site-packages:$PYTHONPATH
````

#### Step 3. install cutadapt
````
pip install --user --upgrade cutadapt
````




