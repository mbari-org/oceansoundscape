---
description: oceansoundscape installation and usage
---
[![MBARI](https://www.mbari.org/wp-content/uploads/2014/11/logo-mbari-3b.png)](http://www.mbari.org) 

**oceansoundscape** is a Python package to assist with analyzing ocean acoustic data. 

The oceansoundscape package currently supports:

🐳 [Generating optimized spectrograms for classification from Band-Limited-Energy-Detections(BLEDS) created in Raven https://ravensoundsoftware.com](/notebooks/BlueASpecGen) for
  
- Blue whale A, B, and D calls 
- Fin whale 20 Hz calls 
- Computing power spectral density (PSD) estimates in 1 second bins

[Example notebook for Blue whale D call classification with PSD](https://github.com/mbari-org/pacific-sound-notebooks/blob/master/docs/notebooks/bluewhales/classify/blueA/PacificSoundClassifyBlueA.ipynb)

## Install
 
```
pip install oceansoundscape
```