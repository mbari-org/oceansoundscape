# Development 

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

## Setting up the poetry environment

To install poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).  Once poetry is installed, you can install the project dependencies by running:

```poetry install```

# Testing

Run the test suite in the poetry environment with:
  

```poetry run pytest```

The expected output should include something like:
```shell
                              (oceansoundscape) 318ms  Thu May 23 19:53:31 2024
============================================================================================================================== test session starts ===============================================================================================================================
platform darwin -- Python 3.11.0, pytest-7.4.4, pluggy-1.5.0
rootdir: /Users/dcline/Dropbox/code/oceansoundscape
plugins: anyio-4.3.0
collected 2 items                                                                                                                                                                                                                                                                

oceansoundscape/tests/test_raven.py .                                                                                                                                                                                                                                      [ 50%]
oceansoundscape/tests/test_spectrogram.py .                                                                                                                                                                                                                                [100%]

================================================================================================================================ warnings summary ================================================================================================================================
../../../miniconda3/envs/oceansoundscape/lib/python3.11/site-packages/librosa/util/files.py:10
  /Users/dcline/miniconda3/envs/oceansoundscape/lib/python3.11/site-packages/librosa/util/files.py:10: DeprecationWarning: pkg_resources is deprecated as an API. See https://setuptools.pypa.io/en/latest/pkg_resources.html
    from pkg_resources import resource_filename

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
========================================================================================================================== 2 passed, 1 warning in 2.45s ==========================================================================================================================```