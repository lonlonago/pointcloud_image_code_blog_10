As a direction of previous research, I have always wanted to find better computational methods, but methods such as the table method and the voxel accumulation method have their own shortcomings, so the AlphaShape algorithm is used to replicate the ideas in the paper to solve the tree crown volume.  

#  I. Introduction 

>  As one of the very classic edge algorithms, in three-dimensional space, 

          a 

         \alpha 

     - 

          s 

          h 

          a 

          p 

          e 

         shape 

     The principle of the shape algorithm is to divide a radius into 

          a 

         \alpha 

     The sphere of alpha is in a finite disordered set of points 

          S 

         S 

     Scroll in S, when 

          a 

         \alpha 

     When the value of α is large enough, the ball will not roll into the interior of the point set, so connecting the points that the circle has rolled through is the point set 

          S 

         S 

     The boundary of S, the set of points 

          S 

         S 

     The concave package of S; when 

          a 

         \alpha 

     If the value of α is small enough, then each point may be a boundary point, as shown in the figure below. Because this paper directly uses the AlphaShape function in MATLAB to calculate the canopy volume, it does not specifically introduce the implementation principle of the algorithm. The details are as follows. 

![avatar]( 8a9bd503beb64700a4c5ba7dbedd48b7.png) 

 ![avatar]( 3ed0622f05ed45beb18406db1b408c60.png) 

#  Second, algorithm implementation 

##  2.1 Ideas 

>  1. Set up the initial 

          a 

         \alpha 

     Alpha value, which can use the point cloud average point spacing as the initial value. 2. Use the AlphaShape algorithm to construct concave packets to determine whether only one area concave packet is generated, if not, update it 

          a 

         \alpha 

     Alpha value, repeat the process of 2 until used 

          a 

         \alpha 

     When the α value generates only one concave packet (this condition is based on the principle of connectivity, using a concave packet to wrap the entire tree), the algorithm stops calculating the volume of the concave packet and outputs the value of the canopy volume. 

##  2.2 Code implementation (MATLAB) 

>  AlphaShapeV1.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574041440
 ```  
>  PointsAverageSpacing.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574041440
 ```  
#  III. Achieving results 

![avatar]( 844ac22a9a7446c8a645a496cdaca17e.png) 

>  In particular, it is stated here that the above process of calculating the canopy volume is just a realization of some of its own ideas, and has not been verified by reasonable results. If you are interested, you can continue to study in depth "~". 

