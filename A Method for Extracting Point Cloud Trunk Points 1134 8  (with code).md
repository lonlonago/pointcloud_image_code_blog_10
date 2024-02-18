#  Overview of the principle 

>  I have read a paper before, and I feel that the idea is very interesting, so I will realize the effect. The specific process is as follows: (1) First, use the eigenvalues of the neighboring point sets to determine whether the point belongs to the trunk or other types of points. (2) Then add the normal vector constraint in the horizontal direction to further eliminate the non-trunk point cloud data. (3) Cluster the remaining point clouds by using the Euclidean clustering method. (4) Determine whether the point cloud is a trunk point cloud by cylindrical fitting for each category of point clouds. 

#  Implementation code 

>  ExtractStem.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574095687
 ```  
>  DrawCylinderV1.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574095687
 ```  
#  III. Achieving results 

![avatar]( 86fa127b572e431d8f3f9bbb834e0374.png) 

 ![avatar]( 4ea57395020041ffa977a18cbd8cc8cf.png) 

>  Note: Due to the inaccuracy of the program for fitting cylinders in MATLAB, sometimes the point cloud part of the trunk cannot be detected. 

#  reference 

>  [1]Non destructive method for biomass prediction combining TLS derived tree volume and wood density 

