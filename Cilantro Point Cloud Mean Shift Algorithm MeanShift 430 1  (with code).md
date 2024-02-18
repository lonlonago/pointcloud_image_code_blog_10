#  I. Introduction 

>  The mean shift algorithm is a very classical hierarchical clustering method, which has been widely used in two-dimensional images. Here we also take two-dimensional images as an example to illustrate its entire calculation process: 

The basic idea of the algorithm: As shown in the figure below, the left side is the distribution of the actual image features, and the right side is the normalized density calculated based on the image feature distribution. It can be clearly seen that there are 7 density peaks on the right side, each of which represents a category center. Therefore, we only need to let each pixel (dot) climb its own mountain, and then find its category. 

![avatar]( d36bb8b5d86d4558bffe637fba7fa405.png) 

 ![avatar]( c5e3c74e11b347efa8a039fc615a1fab.png) 

 After understanding this, the calculation process becomes much simpler. 

>  1. Select a point at random, as shown below, and search for all the points in the neighborhood r of that point. At this time, the neighborhood point set can form a vector set (subtraction), then add it up and take its mean vector, then you can get the second point (green point). 

![avatar]( 1857d3560e74438184ee8e5b8be9a6bb.png) 

>  2. Move the search center to the green point and repeat the process in 1. Finally, the search center will climb to the peak center of the density and mark the point. 

![avatar]( a03733cd57f94ba7bfc5f97c55de45b8.png) 

 ![avatar]( 1f07e4bee0b946f6b4d4b29237526326.png) 

>  3. Traverse all points in the point set and repeat the process in 1-2 until all points are marked, then the algorithm ends. 

![avatar]( 8e700a6f7f1c43239f112698deef67a9.png) 

 Of course, this is the original algorithm. In order to reduce the amount of computation, we can also label all points in each point path to speed up the computation of the clustering process. 

#  Implementation code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573973709
 ```  
#  III. Achieving results 

![avatar]( 118f42e4ddf14e90b15c4f9f73ff0b99.png) 

#  reference 

>  [1]https://www.youtube.com/results?search_query=MeanShift 

