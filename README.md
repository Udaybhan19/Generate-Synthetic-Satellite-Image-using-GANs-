# Generate-Synthetic-Satellite-Image-using-GANs-
## Ultimate goals :
    •	Build a base model from an off-the-shelf implementation
    •	Train it with the chosen dataset, finding a good set of parameters
    •	Discuss possible model predictions 
    •	Extract conclusions about the different improvements attempted.
## The Datasets : 
The data has been taken from the SAS planet satellite image dataset. We are working on the satellite images and maps of Mumbai city and its outside area. We have created a dataset by merging satellite images and their corresponding map images. The whole training set consists of a training set (863 images ) and a test set (174 images ). 
All the images and maps have a resolution of 7424*7424 pixels.

  ![image](https://user-images.githubusercontent.com/90769423/152635409-a58d3d61-93af-409e-86bd-99800d6635ef.png)![image](https://user-images.githubusercontent.com/90769423/152635524-80249c9f-2a9f-4c0b-a49a-7f585976320b.png)




## Related Work : 
Our first steps with the chosen implementation were to understand it, compare it with the original pix2pix implementation and prepare a Jupyter notebook to test the code.
### Required Library :
1.	Tensorflow 
2.	Os 
3.	Time 
4.	Datetime 
5.	Matplotlib
6.	Ipython 
### Accessing the dataset :
1.	First we read the all data file with help of tensorflow and decode it into jpeg file and we visualize one of the image from the data. we get 256*512 size images
2.	The images are then resized to 286x286, transformed into a tensor
3.	Their values get normalized, 
4.	A random 256x256 crop is performed and in half of the times they're flipped . 



### Features Steps :
1.	Now built a input pipeline with tf.data
#### 2. Build the generator :
           Define the generator loss 
#### 3.	Build the discriminat: 
           Define the discriminator loss 
4.	Define the optimizers and a checkpoint-saver 
5.	Generate images 
6.	Training 
7.	Restore the latest checkpoint and test the network 
8.	Generate some images using the test set. 


