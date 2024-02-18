#  I. Introduction 

>  In point clouds, the normal vector and curvature estimation are just geometric representations of the base around a specified point. Although they can be computed quickly, they can represent limited information, so sometimes it is easy to fail to process the data simply by using curvature and normal vector. Therefore, some scholars have proposed new feature descriptors, which can better represent the surface information around points, and PFH (Point Feature Histogram) is one of them. The goal of PFH is to encode the k-neighborhood geometric properties of points by generalizing the average curvature around points using multi-dimensional value histograms, which can handle different sampling densities and neighborhood noise well. 

#  Feature implementation 

##  2.1 Implementation steps 

>  (1) Calculate the normal vector for each point. The characteristic histogram representation of a point is based on the relationship between the points in the neighborhood and their surface normals. Simply put, it attempts to capture the variation of the sampled surface as much as possible by considering the interaction between the normal directions. Therefore, the first step in computing the PFH is to calculate the normal vector for each point. 

>  (2) Calculate the difference between all points within a sphere with a radius of r for each point ( 

          a 

          , 

          b 

          , 

          i 

          , 

          d 

         \alpha,\beta,\theta,d 

     α, β, theta, d). Since you want to represent the information around the point, you need to calculate the difference from the surrounding points. As shown in the figure below, you can calculate the three included angles and the distance between the two points. In this way, a total of 12 values (position + normal vector) of the two points can be compressed to 4 values. 

![avatar]( 57ca74824644488c9612ed1933a91d18.png) 

>  In addition, since this calculation process is performed in pairs at all points in a spherical range, the final PFH descriptor is computed as a histogram of the relationship between all point pairs in the neighborhood, so the computational complexity is 

          O 

          ( 

           k 

           2 

          ) 

         O(k^2) 

     O (k2) (assuming there are k adjacent points). 

![avatar]( 8f115f3969fe4cd69503d6e370819726.png) 

>  (3) Classify statistics. Put all the obtained ( 

          a 

          , 

          b 

          , 

          i 

          , 

          d 

         \alpha,\beta,\theta,d 

     α, β, theta, d) for classification processing, the classification process requires us to classify each point, such as equal spacing division, three angle features, each angle feature is divided into 5 grades, then there are 

           5 

           3 

         5^3 

     53 kinds of combination intervals. Therefore, for each feature, the categories should not be too many, just like our exams, which can be divided into excellent, good, pass, and fail. If there are too many categories, it is easy to increase the probability of error. Then classify the calculated results in (2) one by one, and count the number of each interval, so that the PFH descriptor of each point can be obtained. 

Note: The feature d (distance) is not used in PCL because, in general, the size of d is not directly related to the shape of a plane, corner, cylinder, etc. Therefore, PCL defaults to the absence of d. 

##  2.1 Implementation code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573930976
 ```  
#  III. Achieving results 

Displays a characteristic histogram of three of the points. 

>  overall 

![avatar]( 48a4cd80ad6543ca8020696643afecd4.png) 

>  local 

![avatar]( aede206e85804125b0c6310d0186c310.png) 

#  reference 

>  [1]Semantic 3D Object Maps for Everyday Manipulation in Human Living Environments 

