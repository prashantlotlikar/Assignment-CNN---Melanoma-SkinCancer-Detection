# Project Name
- Melanoma Skin Cancer Detection


# Problem Statement
- Problem statement: To build a CNN based model which can accurately detect melanoma.


# Methodology and results 

## 1. Data Reading/Data Understanding → Defining the path for train and test images
- mount google drive
- unzip the dataset from google drive
- Defining the path for train and test images from google drive
- Count the number of image in Train and Test directory Using the glob to retrieve files/pathnames matching a specified pattern.

-- Count : Train 2239 / Test 118
	
## 2. Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Visualize one instance of all the class present in the dataset.
-- Found 2239 files belonging to 9 classes.


## 3. Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset
- Visualize distribution of classes in the training dataset.

- ![download](https://github.com/prashantlotlikar/Assignment-CNN---Melanoma-SkinCancer-Detection/assets/132319149/a64b1d15-0307-4c43-a4cd-f2b90af2da3d)


## 4. Class distribution: → Examine the current class distribution in the training dataset
- ![download](https://github.com/prashantlotlikar/Assignment-CNN---Melanoma-SkinCancer-Detection/assets/132319149/6075e2e8-fa96-405c-bda4-93ecd58761ee)

-
## 5. Handling class imbalances: → Rectify class imbalances present in the training dataset with Augmentor library.

## 6. Class distribution: → Examine the current class distribution in the training dataset

## 7. Chose an appropriate data augmentation strategy to resolve underfitting/overfitting
- Adding 500 samples per class to make sure that none of the classes are sparse in training dataset
- Count total number of image generated by Augmentor.
-- 4500
-
## 8. Model Building & training on the augmented data :
-- Found 6739 files belonging to 9 classes.Using 5392 files for training.
-- Found 6739 files belonging to 9 classes. Using 1347 files for validation.
-  Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).

- # Plot the training curves
 ![download](https://github.com/prashantlotlikar/Assignment-CNN---Melanoma-SkinCancer-Detection/assets/132319149/49fadeaa-6bc3-4595-adb6-05c9035b72cc)


## 9.0Model Building & training on the rectified class imbalance data
- 1/1 [==============================] - 0s 27ms/step
Actual Class basal cell carcinoma
Predictive Class basal cell carcinoma
