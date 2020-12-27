# TensorFlowLite classifier using Python
Image classifier using Tensor Flow Lite and Python.

Based on https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/examples/python

## Requirements
Python 3.8
Can be used without GPU

## Installation
1. Install Python
2. Update pip

    pip install --upgrade pip

3. Install Tensor Flow (currently installing only Tensor Flow Lite not works for me)

    pip install tensorflow

4. Install Pillow for loading image support
    
    python -m pip install --upgrade Pillow

## Running

To run the classifier, type this:
    python label_image.py
    
If CUDA is not setupm Tensor Flow complains this, but the program works and quite fast:

    ... W tensorflow/stream_executor/platform/default/dso_loader.cc:60] Could not load dynamic library 'cudart64_110.dll'; dlerror: cudart64_110.dll not found
    ... I tensorflow/stream_executor/cuda/cudart_stub.cc:29] Ignore above cudart dlerror if you do not have a GPU set up on your machine.
    0.919720: 653:military uniform
    0.017762: 907:Windsor tie
    0.007507: 668:mortarboard
    0.005419: 466:bulletproof vest
    0.003828: 458:bow tie, bow-tie, bowtie
    time: 54.104ms

At the first run it takes some time to load Tensor Flow, but next it loads faster.
Nethertheless for repetitive image processing consider looping inside the program.

## More models
For more Tensor Flow Lite models for image classification see here:

https://www.tensorflow.org/lite/models/image_classification/overview






