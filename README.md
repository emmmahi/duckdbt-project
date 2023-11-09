# Setting up a virtual environment

Setting up a virtual environment for database using python. Going to use duckDB as database. 

# About python

```bash
# check your python

#version
python --version

#all python paths
where python

#gives one versions path
which python
```

Please notice that python 3.12.0 doesn't work in this project. Use python version 3.11.x.

# How to install dbt

1. First let's choose the right python for out virtual environment.
Replace 'python' with the right path if `which python` doesn't give you the one you want (check the backslash is like this / and not this \ ).
This command creates **.venv file** and now you have python in your project even it would be deleted from your computer.

`python -m venv --copies .venv`

2. Let's activate the virtual environment. You can check that these folders/files are in **.venv-file**.
`source .venv/Scripts/activate`

You can exit virtual environment with command
`deactivate venv`

# Creating some src/playgroung/test.py

`mkdir -p <name/name>` allows to create multiple folders at the same time.
`touch <name>` makes new empty file.

So let's make some new directories and files:`

`mkdir -p src/playgroud`
`touch src/playgroud/test.py`

Open **test.py** file. See in the down right corner, that you are using the right python version and that it says it is virtual environment.

## Creating requirement.txt

Make new file to your root folder.
`touch requirements.txt`

And write this inside it:
duckdb==0.9.*
dbt-duckdb==1.7.*

## Install packages with pip: -r requirements.txt
Use the command below to install the packages according to the configuration file requirements.txt.

`pip install -r requirements.txt`


# Creating new folder dbt_example

This will make new folder under root. 
`dbt init dbt_example1`

See what it includes.


## WHAT NEXT??

1. some modifications to files inside dbt_example1
2. dbt build????









