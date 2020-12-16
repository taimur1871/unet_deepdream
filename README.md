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

### nidek_1 Dataset

In nidek_1 dataset the activations analyzed were in a deeper part of the decoder layer. The darker spots and areas with more variation are represented by embossed areas. The smoother white areas are represented by smoother areas in the pictures.

![Original](https://github.com/taimur1871/unet_deepdream/blob/main/images/original_resized_ndk.png)
![DeepDream 1](https://github.com/taimur1871/unet_deepdream/blob/main/images/deepdream_1_ndk.png)
![DeepDream 2](https://github.com/taimur1871/unet_deepdream/blob/main/images/deepdream_2_ndk.png)

# 2-Layer UNET

The following is a representation of a 2-layer unet model. This model was not very effective at correctly segmenting the images. Especially the cirrus_3 images. It still segmented some images on nidek_1 dataset. The examples are shown below the model description.

![2-Layer UNET](https://github.com/taimur1871/unet_deepdream/blob/main/model_architecture/unet_2layer.png)

## Segmented Images
### cirrus_3

![unet 4layer cirrus segmentation]()
![unet 2layer cirrus segmentation]()

### nidek_1

![unet 4layer nidek segmentation]()
![unet 2layer nidek segmentation]()

# 3-Layer UNET

The following is a representation of a 2-layer unet model. This model was not very effective at correctly segmenting the images. Especially the cirrus_3 images. It still segmented some images on nidek_1 dataset. The examples are shown below the model description.

![3-Layer UNET]()

## Segmented Images
### cirrus_3

![unet 4layer cirrus segmentation]()
![unet 3layer cirrus segmentation]()

### nidek_1

![unet 4layer nidek segmentation]()
![unet 3layer nidek segmentation]()
