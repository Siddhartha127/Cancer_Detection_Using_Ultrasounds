# Cancer Detection Using Ultrasounds


The model we develop is designed to handle images from various sources and classify them according to their clinical significance. The first model aims to distinguish between ultrasound images and 
non-ultrasound images, thereby filtering out irrelevant images and focusing on those that may indicate the presence of cancer. The second model classifies images based on their relevance to breast and 
gallbladder cancer, further narrowing down the scope of analysis.



## Why we introduced this model?


Cancer is one of the major leading cause of death worldwide despite several advancements in the field of technology and medical science. The detection of cancer, especially in its early stages, is proven to be 
very beneficial for the recovery of the patient. However, the process often involves complex procedures and requires skilled medical professionals, making the costly cure challenging to reach remote places 
and poor population.
In light of these challenges, there is an increasing demand for the efficient and accessible diagnostic tools. This is where ourproposed model comes in use.


## Flow of the Model

The model we are proposing introduces a method that uses deep learning to analyze medical photos and extract useful information. The model starts by using a ResNet-50 model to determine if the input picture is an 
ultrasound image or not. If yes, a second ResNet-50 model is used to categorize the organ that the ultrasound picture depicts. The model consists of specialized models for focused cancer detection after 
obtaining this organ identification. For example, a VGG16 model actively looks for breast cancer, while another ResNet50 model looks for gallbladder cancer.

![flw](https://github.com/suyash-dabral/Cancer_Detection_Using_Ultrasounds/assets/159096895/2f016456-b5e6-4e3a-abd6-58b7fed030ca)




## Dataset Used

We utilized different datasets for the development of our models. The first dataset was used for the model designed to identify whether an image is an ultrasound or not. This dataset consisted of a mix of 
ultrasound and nonultrasound images. For the non-ultrasound images, the dataset included a variety of image types such as colored images, X-rays (can be found at Kaggle by bjoernjostein under 
food-classification), and food pictures (can be found at Kaggle by paultimothymooney under chest-xraypneumonia). On the other hand, the ultrasound images included breast ultrasound and gallbladder ultrasound 
images. 
For the second model which was to predict the organ present in the image, we used the dataset which was the combination of all the ultrasound images that required the conversion of labels to a one-hot 
encoded format. Based on the output, the images were classified into two categories: 0 representing breast images and 1 representing gallbladder images. Then for the Breast Cancer Ultrasound detection, 
we used the dataset that can be found at Kaggle by fhabibimoghaddam under breast-ultrasound-images for the models designed to classify images based on their relevance to breast cancer. In this dataset, 
the images were classified into three categories: 0 representing normal images, 1 representing benign images, and 2 representing malignant images.
As for the Gall Bladder Cancer detection, we received the dataset from https://gbc-iitd.github.io/data/gbcu. The dataset is named as GBCU (Gall Bladder Cancer Ultrasound) which is the first dataset 
available to public for Gallbladder Cancer identification with the help of Ultrasound images. This dataset consists of 1255 images in which 432 images are normal, 558 images have benign cancer, and 265 images 
contains malignant cancer. This data is collected from 218 patientsa. Of the 218apatients, 71a, 100a, and 47a were from the normal, benign, and malignant classes, respectively.




## If you want to access the model, visit the below link of the organization:

