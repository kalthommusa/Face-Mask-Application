# Project Objective

Design, train, and test deep convolutional neural networks with transfer learning to perform a face mask classification task with PyTorch and IBM Computer Vision Studio.

----------------------------------------------------------

# CV Studio

When building Computer Vision applications, we deal with a lot of images, videos, and other assets that require storage. Image processing also requires significant computing power. The ultimate goal of every computer vision project is to have it deployed as part of an application and every application requires infrastructure to run.  

[CV Studio](https://vision.skills.network/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkCV0101ENCoursera25797139-2022-01-01/) is a Computer Vision learning tool for building, running, and managing AI Vision computer models and optimizing decisions anywhere on the IBM Cloud. It uses cutting-edge tools like Jupyter Notebook, Watson Machine Learning, Elyra, and more. 

----------------------------------------------------------

# Project steps / pipline:

  * ## 1- Built the dataset

  When gathering data, my goal was to build a diverse database that contains images of people (with or without masks) of different nationalities, races, and with different styles. And I made sure to include some pictures that reflect the Saudi identity (for both women and men)

  Look at the database:

  (mask category) 
  ![](images/dataset-mask.png)

  (no-mask category)
  ![](images/dataset-no-mask.png)

  I collected and uploaded 360 images divided into 180 images of people wearing masks and 180 images of people without masks on their faces.

  ![](images/upload-images.png)

  ----------------------------------------------------------

  * ## 2- Annotate the dataset

  Since I named both of my folders with the respective categories (mask, no_mask) when I uploaded my images in the previous upload step, the annotations happened automatically on CV Studio.     

  And here in the annotate section, I verified that my images are labeled as expected.

  ![](images/annotate-images.png)

  ----------------------------------------------------------

  * ## 3- Train the model

  I chose a Jupyter notebook as a "Training tool" and used the image annotations from the previous step to train a CNN model using transfer learning (using the `ResNet` pre-trained model as a fixed feature extractor) to perform a face mask classification task with PyTorch. 

  ![](images/creating-traning-run.png)

  ----------------------------------------------------------

  * ## 4- Test the model

  To test the classifier, enter the URL of the web app below into any web browser, and enjoy testing the model:

  `
  https://face-mask-application-6364868bf3cbb858b65c1d1a.u8wpmjcrkw2.eu-gb.codeengine.appdomain.cloud/
  `

  Upload or drop & drag an image into the box and the prediction of the deep network will show at the bottom.

  ![](images/the-app.png)

----------------------------------------------------------

# Results & Observations 

By feeding the classifier with 360 images, it has the opportunity to learn and gather enough information about the mask and no_mask data, and understand the relationship between input and output, as a result, the classifier's accuracy is 94% which is very high and promising, and indicates an excellent performance and accurate predictions.

![](images/accuracy.png)


I've tested the app on several images, and the overall performance of the classifier seems pretty excellent.

correct mask1 prediction:

![](images/prediction-1.png)

correct mask2 prediction:

![](images/prediction-2.png)

correct mask3 prediction:

![](images/prediction-3.png)

correct mask4 prediction:

![](images/prediction-4.png)

correct mask5 prediction: 

![](images/prediction-5.png)

correct mask6 prediction: 

![](images/prediction-6.png)

correct mask7 prediction:

![](images/prediction-7.png)

correct mask8 prediction:

![](images/prediction-8.png)

correct mask9 prediction:

![](images/prediction-9.png)

correct mask10 prediction:

![](images/prediction-10.png)

correct mask11 prediction:

![](images/prediction-11.png)

correct mask12 prediction:

![](images/prediction-12.png)

correct mask13 prediction:

![](images/prediction-13.png)

correct mask14 prediction:

![](images/prediction-14.png)

correct mask15 prediction:

![](images/prediction-15.png)

The model made correct predictions and succeeded in classifying all the test images. Therefore, there is no need to retrain the classifier or collect more data.