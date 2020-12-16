# DeepDream Application on Custom UNET

The notebok here explores the idea of applying deep dream to custom unet designed for medical image segmentation.
In addition to that 2 and 3 layer shallow unet models were also created. These were tested on the test images to see how effective these are to segment images.

## DeepDream Outputs

The layer used for this analysis was the second conv layer in the upscale part of the model.
The following three images compare original scan, Deepdream and enhanced DeepDream images. Although very subtle The activation on the enhanced image show the model is already identifying and activating around the cavities.

### cirrus_3 Dataset
![Original](https://github.com/taimur1871/unet_deepdream/blob/main/images/original_resized_cirrus3.png)
![DeepDream 1](https://github.com/taimur1871/unet_deepdream/blob/main/images/deepdream_1.png)
![DeepDream 2](https://github.com/taimur1871/unet_deepdream/blob/main/images/deepdream_2.png)
