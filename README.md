
Problem:

The problem of people not using helmet while driving has caused the increase in number of accidents therefore it is necessary to solve the problem and this can be solved by using machine learning to detect the helmets of the riders both considering the bike riders and bycycle riders. The problem is solved by the method of implementation of CNN layered technique.

Data:

The data was custom made by collecting the images from internet using the online repositories. The data had the diversity and variation to detect any possible kind of scenario of person wearing helment. The data consisted of two classes of person riding the bike and bycycles with helmet and without helmet. The data can be accessed from this link:
https://drive.google.com/file/d/1hxUF7z20tghwRWZiHh7j7qm_uti-030y/view?usp=share_link


Method:

Yolov5 is the most widely used machine learning algorithm for the detection and prediction applications. This project consists of the custom dataset and the annotations were carried out using labalimg toolbox. This model is specifically designed in a manner to detect the bounding boxes for the training and the training of the bounding boxes resulted in prediction of the helmets/no helmets in the project. The bounding boxes of the images were created using the Labelimg toolbox. The dataset used for the project consists of the custom image dataset.

Architecture of the implemented technique can be seen as:

![Seq](https://user-images.githubusercontent.com/116068857/210938172-11ecd036-b0e1-4516-b488-f8acc11ea384.png)

Results:

The results of the given system can be seen as below:

https://user-images.githubusercontent.com/116068857/210938597-becd7e19-095d-47dd-a953-18da1c1bc8e9.mp4

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
             
             
             
 For any queries please contact:
             
             Swathi.kamalapuram@th-bingen.de , faisal.imam@th-bingen.de
