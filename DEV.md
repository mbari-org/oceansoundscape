## Development 

There are two environments in this repository that can be used for development: conda or poetry
 
## Setting up a conda environment
 
This will create an environment called oceansoundscape and make that available in your local jupyter notebook as the kernel named *oceansoundscape*.
Note that the jupyter notebooks are only used for documentation.

```
conda env create
conda activate oceansoundscape
pip install ipykernel
python -m ipykernel install --user --name=oceansoundscape
```


## On MacOS Monterey *may* need to install soundfile and link the libraries
```
brew install libsoundfile
ln -s /opt/homebrew/Cellar/libsndfile//1.0.31/lib/libsndfile.dylib /usr/local/lib/libsndfile.dylib
```

## Install the package in editable mode

```shell
pip install --force -e .
```

## Test

Run the test suite


```shell
nosetests
```

The expected output is 

```shell
----------------------------------------------------------------------
Ran 2 tests in 1.859s

OK
```


## Setting up a poetry environment
 
To install poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).  Once poetry is installed, you can install the project dependencies by running:

```poetry install```

To run the tests, run:

```poetry run pytest```

The expected output is 
```shell
====================================================================================== 2 passed, 1 warning in 3.81s ======================================================================================
~
```