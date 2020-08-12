## Image_Segmentation (Keras)

Masking areas where building are (part of urban-analysis)

Find dataset here: [link](https://drive.google.com/drive/folders/1REaNUpaD6Dm64v1FEDop20LgJtXvorXz?usp=sharing)

Using U-Net model on village finder dataset to maskout areas containing buildings. 
Dataset contains RGB (256x256) images in tiff format, around 3500 training images and around 300 for testing; training set is futher divided into 80-20 ratio for cross-validation to imrprove results. Some data processing is done along the way as well.

#### U-Net Model

U-Net model has 10 Encoder layers and 10 decoder layers (up-sampling to generate image of mask) and some 1x1 conv layers to reduce filter space and give final result image.
Model was quick to learn and within 20-25 epocs it was genrating good results.

#### Results
As model should
![good results](/images/result2.png)

Model trying to narrow it down
![wow results](/images/result3.png)
