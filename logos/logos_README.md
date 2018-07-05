# logos directory README

## Summary
This directory contains logo images that might be used by dynamic kernels listed in the `dynamic_kernels_config.yaml` file. 

## Rules
* The logos should be in png format.
* The logo sizes should be 32x32 or 64x64.
* There can be one logo of each size.
* There doesn't have to be a logo for a kernel.
* The logo filename should be:
    - [language]-32x32.png  or
    - [language]-64x64.png
    - example: Go-32x32.png
    - The language name used in the filename before the dash should exactly match the `language:` parameter in the kernel's corresponding entry in the `dynamic_kernels_config.yaml` file.
* More than one kernel can refer to the same logos if they are for the same language. If, however, the langage parameters are different (e.g. `Python2`  and `Python3`) then each would need its own, appropriately name logo files.
* Logo files that don't correspond to an entry in the config will simply not be used and should cause no harm.

## Other Instructions
When the `dynamic_kernels_config.py` script is run with the `-config` option it will create appropriate directories for each kernel as specified by the `dynamic_kernels_config.yaml` file and copy any available and appropriate logo files into the corresponding directories, renaming them `logo-32x32.png` or `logo-64x64.png`. 


