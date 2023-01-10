Introduction to Object Detection:

Object detection is a computer technology related to computer vision and image processing that deals with detecting instances of semantic objects of a certain class (such as humans, buildings, or cars) in digital images and videos. Object detection algorithms typically leverage machine learning or deep learning to produce meaningful results. The goal of object detection is to detect and classify objects within an image, and to locate the position of the objects within the image.



Object detection is important for a variety of reasons. For example, detecting the bikers who are wearing helmets or not wearing.
Some potential benefits of helmet detection include:

1.Improved safety: By detecting whether or not a person is wearing a helmet, safety systems can alert the user or take corrective action if necessary. This could be particularly useful in industries with a high risk of head injuries, such as construction or cycling.

2.Enhanced compliance: In industries or situations where helmet use is required by law or regulation, helmet detection can be used to ensure compliance.

3.Increased efficiency: In some cases, helmet detection can be used to automate tasks or processes that require the presence or absence of a helmet. For example, a helmet detection system could be used to control access to a construction site or to trigger the start of a manufacturing process.



Object Detection Using Deep Learning:

We can use a variety of techniques to perform object detection. Popular deep learning–based approaches using convolutional neural networks (CNNs), such as R-CNN and YOLO, automatically learn to detect objects within images. One of the most famous families of Deep Convolutional Neural Networks (DNN) for object detection is the YOLO (You Only Look Once).

Object detection pipeline:

![image](https://user-images.githubusercontent.com/116068857/211398429-5834ac83-b39a-4647-8686-ea73609644e2.png)
                         

Problem:

The problem of people not using helmet while driving has caused the increase in number of accidents therefore it is necessary to solve the problem and this can be solved by using machine learning to detect the helmets of the riders both considering the bike riders and bycycle riders. The problem is solved by the method of implementation of CNN layered technique.

Data:

The data was custom made by collecting the images from internet using the online repositories. The data had the diversity and variation to detect any possible kind of scenario of person wearing helment. The data consisted of two classes of person riding the bike and bycycles with helmet and without helmet. The custom object detection dataset (image & bounding box text file) can be accessed from this link:
https://drive.google.com/file/d/1hxUF7z20tghwRWZiHh7j7qm_uti-030y/view?usp=share_link


Method:

Yolo is the most widely used machine learning algorithm for the detection and prediction applications. This project consists of the custom dataset and the annotations were carried out using labalimg toolbox. This model is specifically designed in a manner to detect the bounding boxes for the training and the training of the bounding boxes resulted in prediction of the helmets/no helmets in the project. The bounding boxes of the images were created using the Labelimg toolbox. The dataset used for the project consists of the custom image dataset.

Architecture of the implemented technique can be seen as:

![Seq](https://user-images.githubusercontent.com/116068857/210938172-11ecd036-b0e1-4516-b488-f8acc11ea384.png)

Results:

The results of the given system for a video can be seen as below:

https://user-images.githubusercontent.com/116068857/210938597-becd7e19-095d-47dd-a953-18da1c1bc8e9.mp4

The results of the given system for an image can be seen as below:
![1](https://user-images.githubusercontent.com/116068857/211234266-5a7878ed-0014-4c24-ac46-810b662386f1.jpg)
The results of the given system for an image when noise(salt and pepper) augmentation used can be seen as below:
![salt-and-pepper](https://user-images.githubusercontent.com/116068857/211239414-6728bedc-4ab8-402e-bd04-df765fbf6f95.jpg)



The results of the given system for an image with flip augmentation can be seen as below:
![c158](https://user-images.githubusercontent.com/116068857/211235110-eb523b50-2ca1-45cb-af01-fc8144fda065.jpg)
![c159](https://user-images.githubusercontent.com/116068857/211235144-2e1edc48-ab67-48a8-8c46-d244b8d512fd.jpg)



The confusion matrix of the algorithm can be seen as:
![confusion_matrix](https://user-images.githubusercontent.com/116068857/211157903-1e650141-adb5-4afb-a4ed-e9acf8b0dfa0.png)

The F1 curve can be seen as:
![F1_curve](https://user-images.githubusercontent.com/116068857/211157924-13cc486e-e3d6-4a74-b19c-9f3f29ab497c.png)


The P curve can be seen as:

![P_curve](https://user-images.githubusercontent.com/116068857/211157948-752b76e6-5aa3-42ff-a307-d6e3283f2abd.png)


The PR curve can be seen as:
![PR_curve](https://user-images.githubusercontent.com/116068857/211157954-c37ac29c-ccb3-437d-bc75-31cc913e3edb.png)


The R curve can be seen as:
![R_curve](https://user-images.githubusercontent.com/116068857/211157958-3103b829-8bd3-469e-95fd-5e3561b79ed4.png)

The Labels can be seen as:

![labels](https://user-images.githubusercontent.com/116068857/211157973-06285b30-be37-4fbe-96f1-325527d88bff.jpg)


Overall results are seen as:

![results](https://user-images.githubusercontent.com/116068857/211157963-1d364800-c8ed-42f5-8548-579b248b8cbf.png)

Conclusion:

The problem was solved and the 50 epochs were compiled to finish the training. The trainable parameters were 7015519 parameters, 0 gradients, 15.8 GFLOPs. There were 157 layers in the model and model summary can be seen as:
Model summary: 157 layers, 7015519 parameters, 0 gradients, 15.8 GFLOPs


                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100%|██████████| 25/25 [00:11
                 
                 
                   all        198        420      0.637      0.617      0.676      0.397
                   
                   
                helmet        198        207      0.563      0.773      0.712      0.452
                
                
             no-helmet        198        213      0.711      0.462       0.64      0.343
 
References and Tutorials:

https://www.youtube.com/watch?v=VsZvT69Ssbs&t=159s

https://www.mathworks.com/discovery/object-detection.html

https://www.geeksforgeeks.org/add-a-salt-and-pepper-noise-to-an-image-with-python/

https://www.kaggle.com/code/eneszvo/yolov5-helmet-detection-train-and-inference

https://blog.roboflow.com/yolov7-custom-dataset-training-tutorial/

https://github.com/WongKinYiu/yolov7

https://medium.com/analytics-vidhya/how-to-use-google-colab-with-github-via-google-drive-68efb23a42d

https://www.forecr.io/blogs/ai-algorithms/how-to-train-a-yolov5-object-detection-model-in-google-colab

https://blog.paperspace.com/train-yolov5-custom-data/

https://colab.research.google.com/github/wandb/examples/blob/master/colabs/yolo/Train_YOLOv5_model_on_a_Custom_Dataset_with_Weights_%26_Biases.ipynb#scrollTo=6Rv2ysKDRDM8

https://docs.ultralytics.com/

https://www.youtube.com/watch?v=5h5UtLau3Vc

https://www.youtube.com/watch?v=tgacIcMvqLQ&list=PLcP8bHQl_w-HkHuUBsSUnMr0LXypzov_g

https://blog.tensorflow.org/2021/01/custom-object-detection-in-browser.html#:~:text=Machine%20Learning%20Engineer-,Object%20detection%20is%20the%20task%20of%20detecting%20where%20in%20an,security%20cameras%2C%20and%20autonomous%20vehicles
             
             
 For any queries please contact:
             
             Swathi.kamalapuram@th-bingen.de , faisal.imam@th-bingen.de , mathew.siby@th-bingen.de
