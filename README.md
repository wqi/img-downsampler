# img-downsampler
Simple utility written in Python to automatically apply Gaussian blur and downsample images at different scales (currently 2x, 3x, and 4x) using OpenCV's implementation of bicubic interpolation. This utility can be especially useful in generating training and testing data sets for super-resolution tasks.

## Requirements
* Python 3
* `opencv-python`

## Usage

```
usage: downsample.py [-h] [-k] hr_img_dir lr_img_dir

Downsize images at 2x, 3x, and 4x using bicubic interpolation.

positional arguments:
  hr_img_dir      path to high resolution image dir
  lr_img_dir      path to desired output dir for downsampled images

optional arguments:
  -h, --help      show this help message and exit
  -k, --keepdims  keep original image dimensions in downsampled images
```
