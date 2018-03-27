# Anaconda Usage Memo
And some study materials as time goes by...  

## Installation 
- Insaller from [Anaconda Download](https://www.anaconda.com/download)
- Linux, then  `>> bash ~/Downloads/Anaconda3-4.1.0-Linux-x86_64.sh`
- Confirm installation. `conda -V`

## Virtual Environments 
Python 3.6 environment as "py36"  
`>> conda create -n py36 python=3.6 anaconda`  

Python 2.7 environment as "py27"  
`>> conda create -n py27 python=2.7 anaconda` 

Activate py36 environment (Linux) 
`>> source activate py36` or   
`>> . activate py36`  

Deactivate current environment (Linux)  
`>> source deactivate `

List available environments  
`>> conda info -e`  

## Package installation in current environment 
Install Chainer (as example)  
`>> cnoda install chainer`

Install opencv3 on python3 (Ubuntu).  
*OpenCV on Python3 (e.g., conda install opencv) did not work well, especially to imshow().  The opencv3 is workaround.  
See [This Stack Overflow](https://stackoverflow.com/questions/40207011/opencv-not-working-properly-with-python-on-linux-with-anaconda-getting-error-th)*   
`>> conda install -c menpo opencv3`

## List of pakages installed 
List all packages  
`>> conda list`   

Check version of Chainer  
`>> conda list | grep chainer`

## Uninstall package  
Uninstall Chainer package (as example)  
`>> cnda uninstall chainer`  

## Remove environment  
Remove "py27" environment (as example)  
`>> conda remove -n py27 -all`  

## Shebang in python script file  
For python3  
```
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
```


