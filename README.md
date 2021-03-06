# jackfruit or not a jackfruit

Another fruit based project since I am on a diet! A flann based knn matcher using sift feature extractor and orb detector with a brute force matcher is demonstrated using the training image/ template as the jackfruit.The key points and their descriptors are found using the feature extractors. After which they are feed to the matching algorithms. Different images of fruits are given as an input and the output is shown as a result of feature matches. <br />

From both the algorithms, the features are extracted and the results are stored in the matches/goodmatch variable as a result of a weighted number for each technique. For the training and template image i have used an image of a jackfruit, it being our national fruit! When the feature matching variable returns a certain value it is identified as a jackfruit. <br />

# Dependencies 

I have used the following dependencies.

   * openCV
   * matplotlib
   * numpy
   
# Template

For the training image for KNN and the template for BFMatcher I have used the following image. <br />

![alt-text-2](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/test_images/train.png "title-1")<br />

# Results

For the KNN matcher the minimum match count is 195 and for the brute force matcher it is 10. In case of KNN, matches above 195 is classified as a jackfruit. And for brute force, matches above 10 is idenfied as a jackfruit. Below are the results for different input images in which both the techniques are applied and results are compared which show the match scores.

Flann Based KNN Matcher (match>10 is jackfruit)             |  Brute Force Matcher (match>195 is jackfruit)
:-------------------------:|:-------------------------:
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_1.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_1.png) 
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_2.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_2.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_3.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_3.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_4.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_4.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_5.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_5.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_6.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_6.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_7.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_7.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_8.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_8.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_9.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_9.png)
![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/knn/Figure_10.png) |  ![](https://github.com/hasibzunair/casual-classifier-KNN-BFMatch/blob/master/bfMatch/Figure_10.png)   
<br />

# Resources

Some of the materials are used from the documentations [here](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html), [here](https://thecodacus.com/object-recognition-using-opencv-python/#.W5fw3jFxXIU) and [here](http://www.coldvision.io/2016/06/27/object-detection-surf-knn-flann-opencv-3-x-cuda/). Also I took extensive help from [this](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_table_of_contents_feature2d/py_table_of_contents_feature2d.html) section of the documentations.


