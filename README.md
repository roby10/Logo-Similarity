# Logo-Similarity

Create a Logo Search engine using pretrained features of networks traind on ImageNet.

Dataset used : subsample of Logo-2k+ [download](https://github.com/Wangjing1551/Logo-2k-plus-Dataset) /  [paper](https://arxiv.org/abs/1911.07924)



Networks:

VGG16 - 512 vector dimension

Densenet161 - 2208 vector dimension

Resnext50 - 2048 vector dimension

MobileNet - 960 vector dimension

We use PCA for dimensional reduction [512, 2208, 2048, 960] -> feature vector of dim 50

For any query Q we get 5 similar logos and their distances to the original image using NearestNeighbors algorithm from sklearn.

## Results 
Each col is a networks type used, each row > 1 is a similar logo and it's distance

![results](https://github.com/roby10/Logo-Similarity/blob/main/download3.png)

