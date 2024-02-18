#  I. Introduction 

>  Among many clustering methods, the K-Means clustering method belongs to "prototype-based clustering" (also known as prototype clustering), which assumes that the clustering structure can be characterized by a set of prototypes and is very commonly used in real-world clustering. Usually, this type of algorithm will initialize the prototype first, and then iteratively update the prototype to solve it. Using different prototype representations and different solution methods will also produce different algorithms. 

As a classic "prototype clustering" algorithm, the prototype of the K-Means algorithm is "K cluster centers", and the iterative solution is based on the degree of change of the "centroid" (the average value of the x, y, and z coordinates of all points of the same class) solved by two adjacent solutions. This may also be the origin of the name of K-Means clustering: K cluster centers + centroid (coordinate average value). 

#  Second, the algorithm steps 

>  1. Initialize the prototype, that is, specify the K value and K cluster centers. The designation of cluster centers can be artificially entered, randomly selected, or in other ways, but try to ensure that the distance between cluster centers is not too close. 2. Clustering. Traverse all data points, calculate the distance from each data point to the K cluster centers (I choose the Euclidean distance here, or I can choose the Mahalanobis distance or other distances), and assign each data point to the category of the cluster center closest to the point until the last data point. 3. Update the cluster center. That is, calculate the centroid of each class, and compare the calculated cluster center with the previous cluster center. If all the cluster centers do not change, stop; if there is a change, the current cluster center is used as the new cluster center, and the above process of 2 and 3 is repeated until all the cluster centers do not change. 

#  III. Implementation code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573913578
 ```  
#  IV. Achieving results 

![avatar]( 2046fad5e099412d8623a52a087d49e0.png) 

#  reference 

>  [1] Open3D point cloud K-means clustering (KMeans) 

