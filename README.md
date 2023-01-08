# Data_Augmentation_Using_Keras
This Repository Has Step-wise Flow For Data Augmentation Using Keras

## Data Augmentation
In this repository, a simple yet effective method to build a powerful image classifier, using only very few training examples is shown, where few images is transformed into a multi image dataset.

## Steps Involved

1. Collect images in a folder
2. Augment the images and store in another folder in same working directory
3. Combine the images into a single folder

## Walkthrough

### Collect Images

I collected three personalities images, J K Rowling, Indra Nooyi and Michael Malarkey and saved them in documents directory
![image](https://user-images.githubusercontent.com/71513343/211204491-2cba764e-1655-404c-a64b-38edf215e417.png)
JK folder images count - 10--

![image](https://user-images.githubusercontent.com/71513343/211205684-71d0307e-e214-4399-9f65-e41c992771af.png)


## Jupyter Node Book Coding

open the notebook file given in the repository 
> Install the required libraries keras, tensorflow using pip install command

execute the code cells and modify the file path as per your file location and naming
***Note:*** The file access and saving directory must be in the working directory (The place where your notebook file is stored is called working directory, in my case it's Documents)

```
img = load_img('C:/Users/indus/Documents/Indusha Images/JK/10.jpg')  # this is a PIL image

```

over here the "10.jpg" is the image name and for each image it is recursively changed to next file name to run manually.

```
for batch in datagen.flow(x, batch_size=1,
                          save_to_dir='JKR', save_prefix='JK', save_format='jpeg'):
```
All the augmentented images are stored in the JKR folder in my instance

## Image Integration

Combine the JK images and JKR images to obtain with more than 308 images with just 10 images--

![image](https://user-images.githubusercontent.com/71513343/211205749-bd5b5984-1e01-4d78-b14c-74f7fb463c67.png)



## Further Learning

To view the construction of a image classification model with the above image data, proceed to the below link.



*Thank you for reading!*
