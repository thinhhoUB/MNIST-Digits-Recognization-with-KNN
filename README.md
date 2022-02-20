# MNIST-Digits-Recognization-with-KNN

Recognizing Digits with KNN using public MNIST database 

by Thinh Ho

## Motivation
After finishing my first project about EDA, I continue to practice my Python knowledge alongside with learning Machine Learning. In order to reinforce the knowledge and get my hand dirty, I choose the MNIST database to practice. Despite it is widely used as a project ideas, my approach is different as I develop my own KNN algorithm and explore deeper the insight of the outcome. 

## 1) Project Introduction
Going to the websit **http://yann.lecun.com/exdb/mnist/**, I download the database include 60 000 images and labels to get ready for my project. Throughout my project, I will :

> - Develop KNN algorithm
> - Investigate performance of model
> - Insights about the final results

## 2) Project Detail
As part of the algorithm, I come up with two different function:
> - First one using Eucledian formula to calculate the distance
> - Second one using Manhattan formula

The purpose is to compare which method will yield the better accuracy rate at the end.

Next step, I try to answer question how numbers of training data and numbers of neighbors will affect the accuracy. Here is the result :

![image](https://user-images.githubusercontent.com/80074386/154861582-ee2860e3-45d9-4b96-95a4-62aae7a09c74.png)

Especially, out of 300 images using for testing, up to 82.35% of them that are perfectly classified (all their neighbors have the same labels). On the other hand, there are 2 images that are not classified correctly even all the neighbors have the same labels.

Lastly, I develop a confusion matrix from stratch to understand better which numbers are most difficult to recognize and being confused most with which numbers:

![image](https://user-images.githubusercontent.com/80074386/154861736-bc4424b6-7d41-4cd0-a87a-e0171f16b8a3.png)

## Conclusion

In conclusion:

> - k-NN algorithm works really well for the MNIST database.

> - Overall, using **Eucledian** distance yields better accuracy rate than using **Manhattan** distance (numbers of neighbors are equal).

> - For both of the method, giving a **higher training dataset** will result in the **better accuracy rate** at the end.

> - However, as the numbers of **neighbor increase**, the **accuracy rate** will be **decreased**. 

> - Using **7000 training** images and **300 testing** images, we achieve **96.3% accuracy** which means around **289 images** are correctly classified.

> - In those 289 images, **82.4%** of them that are **perfectly** classified ( all the neighbors have same label).

> - There are **2 outliers** which are incorrectly classified despite all the neighbors have same label.

> - From 0-9, number **8** is the most confused and it is mainly misclassified as number **5** and **9** instead.
