# Blob Segmentation with U-Net

`Status`: passed

`@author`: Ali Hashmi

`@note`: The python script uses `MXNET` (a modern opensource deep learning framework) to implement U-net: https://lmb.informatik.uni-freiburg.de/people/ronneber/u-net. You may need to install all the appropriate libraries/modules for python: mxnet (configure it for GPU), opencv etc.. As of now, the script has only been tested on Windows.
(1) Download the script files to the same folder (2) Provide the folder path to `sys.path` or add the folder path to PYTHONPATH in the environment variables of your system.

The neural network is general purpose. Please modify and/or customize the scripts for your segmentation problem (possibly it requires the search for new hyperparameters)

The convolutional neural network (`CNN`) was trained sufficiently - the training-dataset consists of images and labels - over an Nvidia GTX 1050 GPU (640 CUDA cores). The training takes a matter of a few minutes. Training over CPU is possible in case a GPU is not available, albeit it will take a considerably longer period (usually several hours due to a lower number of processor cores).

The neural-network once trained can be applied on an image to generate the segmentation mask

### Example:

![alt text](https://github.com/alihashmiii/blobsegmentation/blob/master/for%20readme/unet%20python.png)




`To do`: 
- resize output back 
