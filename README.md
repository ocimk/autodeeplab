<!-- <a href="https://doi.org/10.5281/zenodo.1248776"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.1248776.svg" alt="DOI"></a> -->

# Vehicle background removal using DeepLab Image Semantic Segmentation Network

For this demo, we used deeplab package available [here](https://github.com/sthalles/deeplab_v3). The description of the Semantic Segmentation is detailed here [Rethinking Atrous Convolution for Semantic Image Segmentation](https://arxiv.org/pdf/1706.05587.pdf).

## Dependencies

- Python 3.x
- Numpy
- Tensorflow 1.9.0
- OpenCV 3.4.1
- deeplab_v3

## Downloads

### Images

Place all images with jpeg extension inside `images` folder. If the folder **does not** exist, create it. You need to modify the folder path in **CreateTfRecord.ipynb**.

### Deeplab
Place deeplab package available [here](https://github.com/sthalles/deeplab_v3) inside `./deeplab_v3`. If the folder **does not** exist, create it.

### ResNet Model
- [checkpoints](http://download.tensorflow.org/models/resnet_v2_50_2017_04_14.tar.gz)

Place the checkpoints folder inside `./deeplab_v3/resnet`. If the folder **does not** exist, create it. checkpoints folder should contain files with .graph and .ckpt extensions. 

### Pre-trained model.

- [checkpoints](https://www.dropbox.com/sh/s7sx69pqjhrk0s4/AACXWCRd9JJ0zvcvDES9G3sba?dl=0)

Place the checkpoints folder inside `./deeplab_v3/tboard_logs`. If the folder **does not** exist, create it.

## Evaluation

### Create TFRecords

Run the jupyter notebook **CreateTfRecord.ipynb** to convert all of the jpeg images to one file with TFRecords extension that is a standard format for tensorflow.

### Test the model on your data

Run the jupyter notebook **deeplab_background_removal.ipynb** to evaluate the pretrained model on the image dataset.

## Results

- Example of processed images without any transfer learning

![Results1](/processed_images/01.png)

![Results2](/processed_images/02.png)

![Results3](/processed_images/03.png)

![Results4](/processed_images/04.png)

![Results5](/processed_images/05.png)

![Results6](/processed_images/06.png)

![Results7](/processed_images/07.png)

![Results8](/processed_images/08.png)

![Results9](/processed_images/09.png)

![Results10](/processed_images/010.png)

![Results11](/processed_images/011.png)

![Results12](/processed_images/012.png)

![Results13](/processed_images/013.png)

![Results14](/processed_images/014.png)

![Results15](/processed_images/015.png)

![Results16](/processed_images/016.png)

![Results17](/processed_images/017.png)

![Results18](/processed_images/018.png)
