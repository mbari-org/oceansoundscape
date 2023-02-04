[![MBARI](https://www.mbari.org/wp-content/uploads/2014/11/logo-mbari-3b.png)](http://www.mbari.org)

[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
![Supported Platforms](https://img.shields.io/badge/Supported%20Platforms-Windows%20%7C%20macOS%20%7C%20Linux-green)
![license-GPL](https://img.shields.io/badge/license-GPL-blue)

# About

A python package for analyzing ocean acoustic data. 
 
Author: Danelle Cline, [dcline@mbari.org](mailto:dcline@mbari.org)

## Prerequisites
 
- Python 3.8 or 3.9
 
## Installation

```pip install oceansoundscape```

## Documentation

Full documentation is available at [https://docs.mbari.org/oceansoundscape/](https://docs.mbari.org/oceansoundscape/)

## Upgrading to version 2.0

If you are upgrading from a release prior to 2.0, the only change needed is to modify

```
from oceansoundscape.spectrogram import conf
blue_a_conf =  conf.CONF_DICT['blueA']

low_freq = blue_a_conf['low_freq']
high_freq = blue_a_conf['high_freq']
```

to 

```
from oceansoundscape.spectrogram import conf
blue_a_conf =  conf.CONF_DICT['blueA']['freq_range'][0]

low_freq, high_freq = freq_range
``` 
