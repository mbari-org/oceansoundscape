---
description: oceansoundscape installation and usage
---
[![MBARI](https://www.mbari.org/wp-content/uploads/2014/11/logo-mbari-3b.png)](http://www.mbari.org) 

**oceansoundscape** is a Python package to assist with analyzing ocean acoustic data. 

The oceansoundscape package currently supports:

🐳 [Generating optimized spectrograms for classification from Band-Limited-Energy-Detections(BLEDS) created in Raven https://ravensoundsoftware.com](/notebooks/BlueASpecGen) for
  
- Blue whale A, B, and D calls 
- Fin whale 20 Hz calls 

Computing power spectral density (PSD) estimates in 1 second bins

## In development 🚧

-  Tutorial on training a CNN classifier with optimized spectrograms

## Potential roadmap

-  Generating standard products using [PyPam](https://github.com/lifewatch/pypam) in AWS. 

## Install
 
```
pip install oceansoundscape
```

Install and update using [pip](https://pip.pypa.io/en/stable/getting-started/) in a Python>=3.8.0 or < 3.10 environment:

```shell
pip install -U oceansoundscape
```
 