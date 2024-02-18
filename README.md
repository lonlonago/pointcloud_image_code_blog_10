##  0. Task Description 

##  1. Load to display the original point cloud 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
![avatar]( 27f517cf21354152bf4151085895d23c.png) 

##  2. Point cloud preprocessing 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
![avatar]( 677ff0df011b4a54a0b501bf75dad808.png) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  3. Build a learning model 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  4. Train the model 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  5. Scatter calculation of three-dimensional circles and axes 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  6. Visual rendering and new point cloud saving 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  7. Final Effect 

##  8. Complete code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
##  9. Package and release the exe executable file 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574033597
 ```  
![avatar]( 3dec40d7b37740a49d5c89d71cde7573.png) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  Overview of the principle 

>  The specific idea of this method is very simple and ingenious. The specific calculation process is as follows: (1) randomly generated k initial seed points; (2) determine the minimum spacing between each seed point 

          d 

          m 

          i 

          n 

         dmin 

     Dmin (3) if 

          d 

          m 

          i 

          n 

         dmin 

     Dmin is greater than the interval threshold we specified 

          d 

         d 

     D, then proceed to the next step, otherwise repeat the process of (1)~ (2) to regenerate a new seed point. 

#  Implementation code 

>  InitSeed.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957406999
 ```  
#  III. Achieving results 

>  When the interval threshold minDist = 0.5: 

![avatar]( 2a3b7d275f4843ebaad8e81cbc294317.png) 

 It can be seen that several categories of segmentation are incorrect. 

>  When the interval threshold minDist = 1: 

![avatar]( 2ef27f1228664c30b88b09ecc4975be4.png) 

>  Until the interval threshold minDist = 3: 

![avatar]( 710cb76d91574e98803d8695606582bb.png) 

>  At this point, the categories are not only clustered correctly, but also the number of iterations is greatly reduced. 

![avatar]( 5c755bd0a9884936a5b3ada6708f5622.png) 

#  References 

>  [1] Research on key technologies for inspection of airborne laser point cloud transmission lines 



--------------------------------------------------------------------------------

#  I. Introduction 

>  Because I have read an article about using normal vector for point cloud segmentation before, the formula is shown below, which is a bit interesting, so I will take a look at the effect. The idea is also relatively simple, that is, according to the difference between the adjacent point and the current point normal vector average to compare with the threshold we set in advance. If it is greater than this threshold, it belongs to one type of ground object, and vice versa, it belongs to another type of ground object. Since there is no data at hand, I tested it with the example data in PCL. 

![avatar]( 561efe6cce5e458cb7579f3b39f81a59.png) 

 ![avatar]( 500754ee727b49eaa2f9b72e3de89797.png) 

 ![avatar]( 3acc1683c25c4d1fb1efe40fbfa27bc8.png) 

#  Code implementation 

>  main.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574084125
 ```  
![avatar]( b00e217563ed4a8d91ec845d1ea3de21.png) 

 Achieve the effect:  

![avatar]( 359d4449230d4da084103d8e91ed4ff2.png) 

![avatar]( b981a4a40b5149f58044032f60cc9376.png) 

![avatar]( 81f87e62c2cd43fbac1b9c4d347b9a66.png) 

#  III. Modification (another test) 

>  Out of curiosity, I modified the code again to see the effect by fixing the number of neighboring points. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574084125
 ```  
![avatar]( a278deb26564470da2098fe6d2537517.png) 

 Achieve the effect:  

#  IV. Summary 

>  From the implementation point of view, the use of normal vector for point cloud segmentation may indeed be effective for some data, such as the table above can extract its plane. In addition, it should be noted that the difference range mentioned in the paper should not be [0,1], the paper should be divided by 2 after the difference between the two normal vectors, so as to ensure that the average difference is between [0,1], which I thought for a long time to determine, and also refer to the similar algorithm in PCL, if there are any errors, I hope you can help me point out ha "~". 

>  Reference: [1] https://pcl.readthedocs.io/projects/tutorials/en/latest/don_segmentation.html#don-segmentation 



--------------------------------------------------------------------------------

#  I. Introduction 

>  After obtaining the result of the accumulator, we need to analyze the accumulator to obtain the parameters we want, that is, locate the maximum value in the accumulator array, which usually uses two methods: threshold method and non-maximum suppression method. 

>  Among them, the basic principle of the threshold method is: first, set the threshold of the accumulator, and then compare each unit in the accumulator. If it is less than the threshold, it is assigned 0, and vice versa, there is no change, so that a large number of useless parameters can be eliminated. Finally, we can use the morphological closing operation to merge discrete points into regions, and the centroid of each region is our final parameter target. 

>  Non-maximum suppression: This method is implemented by determining whether the value of each cell is higher than the value of all its neighbors. It can retain most of the local maximum values, and it is usually better used with threshold methods. 

#  Code implementation 

>  Threshold method 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957402915
 ```  
>  non-maximum suppression 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957402915
 ```  
#  III. Achieving results 

>  Threshold method 

![avatar]( 8d55489ef6c74bdf9940b56f50f072ab.png) 

>  non-maximum suppression 

![avatar]( c37fbcd580c04f8cbc60f0a8fc3d45a5.png) 

#  References 

>  [1]Principles of Digital Image Processing 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  Overview of the principle 

>  (1) Using the method in the initial segmentation center selection model based on voxel, we first select the initial clustering center (improvement). (2) Using the method of kmeans clustering to cluster point cloud data, the specific principle of kmeans clustering has been introduced in detail in the previous article (point cloud K-Means clustering algorithm), here is the code directly. 

#  Implementation code 

>  KMeansStart.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957408968
 ```  
>  KMeans.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957408968
 ```  
> 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957408968
 ```  
#  III. Achieving results 

![avatar]( 037143822f2f45f3a081d70da0e833a1.png) 

![avatar]( 5450531ca7bc4b83b69f8bf2e85a2e67.png) 

#  References 

>  [1] Research on key technologies of 3D discrete point cloud data processing 



--------------------------------------------------------------------------------

#  Overview of the principle 

>  References have been placed at the end of the article. The algorithm is divided into three stages in total: (1) Create a minimum elevation surface from the point cloud data. Project the point cloud data onto the xy plane and divide it into a grid, then find the lowest elevation (Zmin) value for each grid element, combine all the Zmin values into a 2-dimensional matrix, and then create a surface based on the minimum elevation. (2) Split the surface into ground and non-ground mesh elements. Apply a morphological open operation (corrosion expansion) on the surface, do this with a square structural element with a radius of 1 pixel (described in MATLAB), and then calculate the slope between the minimum surface and the open surface map on each grid element. If the difference is greater than the elevation threshold, the mesh is classified as a non-terrestrial mesh. Repeat the above process, increasing the radius of the structural element by 1 in each iteration until it reaches the maximum radius we specify. The end result of the iterative process is a binary mask mesh where each mesh is classified as terrestrial or non-terrestrial. (3) Segment the original point cloud data. Apply a binary mask on the original minimum surface map to remove the non-terrestrial mesh. Image interpolation techniques are used in the original text to patch the unfilled mesh to create an estimated elevation model (this step is not done in this paper, mainly due to a lack of knowledge about image interpolation techniques). Calculate the elevation difference between each point in the original point cloud and the estimated elevation model. If the difference is greater than the height difference threshold we set, the grid is classified as non-terrestrial. At this point the whole algorithm ends. 

#  Implementation code 

>  MorphologicalFilteringV1.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574093373
 ```  
#  III. Achieving results 

![avatar]( 76e47146f99c45988b29c606674aece2.png) 

#  References 

>  [1]An Improved Simple Morphological Filter for the Terrain Classification of Airborne LIDAR Data. 



--------------------------------------------------------------------------------

#  I. Introduction 

>  Here we use a window to select the lowest point in the window as the ground point. Drawing on the idea of greedy projection triangulation in PCL, we first obtain the ground point and project it to the horizontal plane, and then use the triangulation function in MATLAB to construct a spatial triangulation network. 

#  Implementation code 

>  DelaunayV1.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574038477
 ```  
#  III. Achieving results 

![avatar]( 1b0d62b7305b4b97a3ed57a5bd8e7051.png) 



--------------------------------------------------------------------------------

#  I. Introduction 

>  The specific principle can be found in: Matlab CSF ground point filtering (plug-in). 

#  II. Compilation process 

>  1. Open the cmake tool and specify the source directory and the build directory path. 

![avatar]( f27930cf4d5a46bd9af65420aaa1fc2f.png) 

 Set our installation path by CMAKE_INSTALL_PREFIX 

>  2. Open CSF's VS project, generate a static library, and install it. 

![avatar]( 116ef865435541ac810a5032c8cfc9cb.png) 

 error 

![avatar]( a798f51f974a4a8c8375d3cd2802753d.png) 

 Solution: Remove all other options. The reason for this error should be that the system used by the author is not a Windows system. 

![avatar]( 84d7d255683c4f359e85607b20e53d94.png) 

>  3. The final generated result. 

![avatar]( eafed8f8afe340d78c06a633b6b93f9c.png) 

#  III. Implementation code 

![avatar]( 2d046cf76a6e46dda6ebe1801e0123ff.png) 

>  CMakeLists.txt 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573947439
 ```  
>  mian.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573947439
 ```  
#  IV. Achieving results 

![avatar]( 023d5fdc238643778dc07600728bd576.png) 

 ![avatar]( 9ca5d3be4a9f41b597bbee8a99c3c036.png) 

#  V. References 

>  [1] Matlab CSF ground point filtering (plugin) 



--------------------------------------------------------------------------------

#  I. Introduction 

>  Among the many file formats for storing point clouds, some are "tailor-made" for point cloud data, and some file formats (such as computer graphics and 3D models in computer science or communication data files) have the ability to represent and store point clouds, and are applied to the storage of point cloud information. After years of development, the las file format has gradually become the industry standard format for LiDAR data. The format aims to provide an open format standard that allows different hardware and software providers to output interoperable unified formats. It is a binary file format. There are also some libraries that can read las data, such as the famous lastool, but in fact, the structure is not complicated, and we can easily read and write to the format ourselves. 

Here is a brief description of the format of Las: the data is mainly divided into two parts of information, header information and point data information. Here, take the Las1.2 version of the data as an example, as shown in the following figure: 

![avatar]( 9533ea9bdf2e410481ace7099dc5ecf7.png) 

 ![avatar]( cbd86afd5efc4884a3841eb1e8661cd6.png) 

 After understanding this, it is easy to read the data. For details, please refer to the following code. 

#  Implementation code 

>  LasInput.h 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573988597
 ```  
>  LasInput.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573988597
 ```  
>  main.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309573988597
 ```  
#  III. Achieving results 

![avatar]( 2156c72574fa4196ac9c0ead38c290eb.png) 

 ![avatar]( 86341d5ec30c45b3bb1f3c8155e9314e.png) 

 ![avatar]( 19c9c142523f4baca8631e0fef33da61.png) 

#  reference 

>  [1]https://download.csdn.net/download/dayuhaitang1/87348556 



--------------------------------------------------------------------------------

As an important parameter of trees, the projected area of canopy has a certain influence on the estimation of tree growth and three-dimensional green volume. According to the ideas in this paper, the convex hull algorithm is reproduced and the projected area of canopy is calculated. The specific process is recorded here.  

#  I. Introduction 

>  The convex hull is a concept in geometric graph theory in computers. As an important tool for object shape description and feature extraction, it has been widely used in the research fields of computer graphics, image processing and pattern recognition. Its mathematical description is: In a real vector space V, for a given set X, the intersection S of all convex sets containing X is called the convex hull of X. As seen in the following formula: 

>  The convex hull of X can be used with all points in X. 

           x 

           1 

          , 

           x 

           2 

          , 

          … 

          , 

           x 

           n 

         x_1,x_2,…,x_n 

     A linear combination of x1, x2,..., xn) to build. In a two-dimensional plane, we can think of the convex hull as a stretched rubber band that just encloses the dwelling point, as shown in the figure below: 

![avatar]( 8281a17ae8194ca5af3da3508e3482ca.png) 

>  There are many algorithms for generating convex hulls for planar point sets. The classic algorithms include the Jarris method, the Graham method, and the divide-and-conquer algorithm. Later in this article, we will implement the more widely used Graham convex hull algorithm, which was invented by the mathematician Graham in 1972. 

#  Graham convex hull algorithm steps 

>  1. Find the point with the smallest value of y 

           y 

            m 

            i 

            n 

         y_{min} 

     Ymin, with this point as the starting point. 2. Sort. With 

           y 

            m 

            i 

            n 

         y_{min} 

     The ymin point is the basis point, and all other points in the point set are sorted from small to large according to the horizontal angle, and the sorted point set is obtained 

          P 

         P 

     P, as shown in the figure below. 

![avatar]( 7b70971a371b42b5b305f15e9dbcd7bb.png) 

>  3. Build a baseline. with 

           y 

            m 

            i 

            n 

         y_{min} 

     YMIN and 

           P 

           1 

         P_1 

     P1 builds the initial baseline, adding two points to the convex hull point set 

          c 

          o 

          n 

          v 

          e 

          x 

         convex 

     In convex. Determine subsequent points by crossing products 

           P 

           i 

         P_i 

     Is Pi at baseline? 

           y 

            m 

            i 

            n 

           P 

           1 

         y_{min}P_1 

     On the left side of YMIN P1, build a new baseline 

           P 

           1 

           P 

           2 

         P_1P_2 

     P1 P2, and will 

           P 

           2 

         P_2 

     P2 added to 

          c 

          o 

          n 

          v 

          e 

          x 

         convex 

     In convex, continue to judge subsequent points in the same way 

           P 

           i 

         P_i 

     The positional relationship of Pi to the new baseline, if at the baseline 

           P 

           1 

           P 

           2 

         P_1P_2 

     The left side of P1 P2 will 

           P 

           i 

         P_i 

     Add Pi to 

          c 

          o 

          n 

          v 

          e 

          x 

         convex 

     Convex, and vice versa, if at baseline 

           P 

           1 

           P 

           2 

         P_1P_2 

     The right side of P1 P2, then 

           P 

           2 

         P_2 

     P2 will be available 

          c 

          o 

          n 

          v 

          e 

          x 

         convex 

     Deleted in convex, 

           P 

           i 

         P_i 

     Pi will be added to create a new baseline 

           P 

           1 

           P 

           i 

         P_1P_i 

     P1 Pi. Repeat the above process until all points have been traversed and the algorithm ends. As shown in the figure below. 

![avatar]( 296eb2e81c41413fa2a37ca7577001ed.png) 

>  4. Using this algorithm, a convex polygon is finally obtained, and then the projected area of the canopy can be obtained by calculating the discrete Green's formula (see Equation 3). The calculation formula is: 

![avatar]( b319571f144d4d5f9c7e68ee43fcfeb7.png) 

#  III. Code implementation (MATLAB) 

>  CrossProduct.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075460
 ```  
>  PolarAngle.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075460
 ```  
>  Graham.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075460
 ```  
>  ProjectionArea.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075460
 ```  
![avatar]( 0af94781f92740ad9505a9d4bd72774b.png) 

 Achieve the effect:   

#  IV. Summary 

>  As a relatively simple method for solving the projected area of the canopy, the convex hull algorithm has the characteristics of speed (algorithm complexity is O (nlogn)) and ease of programming. However, the convex polygon obtained by this method can be clearly seen that it is not realistic enough and natural, and there are many gaps, as shown in the figure below, so many papers have used other methods to solve the projected area of the canopy, such as the alpha shape algorithm. 

![avatar]( fca7d685da9445ca9226ef6ccf57aea8.png) 

>  Reference: [1] An automatic extraction algorithm for single tree crown projected area and crown volume based on 3D laser point cloud data [2] "Introduction to Algorithms - Finding Convex Hulls" 



--------------------------------------------------------------------------------

#  I. Introduction 

>  In computer graphics, convex hull refers to the smallest convex set containing a finite point set P in any dimensional space. It is composed of convex hull vertices, which appear as a convex polygon in two dimensions, and a convex polyhedron in three dimensions. At the two-dimensional level, the most commonly used convex hull algorithms are Graham scanning method and Jarvis volume wrapping method, but the former is not suitable for three-dimensional level, while the latter can be extended to three-dimensional. In addition, at the three-dimensional level, convex hull algorithms include Clarkson-Shor and QuickHull, both of which are incremental methods, but the latter is more commonly used in practical applications and is a very good convex hull algorithm. The convex hull algorithm in PCL and MATLAB adopts QuickHull algorithm. The convex hull has been used in many fields. In this paper, the convex hull algorithm is used to calculate the volume and surface area of the crown convex hull. 

#  Second, code implementation (MATLAB) 

>  TrdDConvexHullV2.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075354
 ```  
> 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574075354
 ```  
#  III. Achieving results 

![avatar]( e0d777a1a96644cf91c635fad16062b0.png) 

![avatar]( 1c0200ef1c6643a8b4d077be0c811ba5.png) 

![avatar]( 629eb6fd6eb64b438371683b4ac34f74.png) 

 Adjust the color and it will look much better.  

>  References: [1] The quickhull algorithm for convex hulls [2] Automatic extraction of tree measurement factors based on point cloud data 



--------------------------------------------------------------------------------

>  When you treat the world fiercely, the world becomes gentle 。 ------ Yu Hua 

#  I. Introduction 

>  I saw such a method for slicing in the paper before. The specific process is as follows: 1. First, perform isometric stratification according to the specified number of layers. 2. Calculate the projected area of each layer of point cloud. 3. Calculate the area ratio between adjacent layers and calculate the average value of all ratios. 4. Classify point cloud slices larger than the average ratio into one category, and vice versa into another category. 5. Compare whether adjacent point cloud slices are of the same type, and merge if they are of the same type, otherwise they will not be merged. 

#  Code implementation 

>  Drawing.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574096374
 ```  
#  III. Achieving results 

![avatar]( 78695923412d45018905f1a55ae374ae.png) 

![avatar]( 5c125bf512f740e397f5a16e46c0e33e.png) 

![avatar]( 6e2a9c0800154a388262a706f3f11f01.png) 



--------------------------------------------------------------------------------

#  I. Introduction 

>  This method was first proposed by Omasa et al. to calculate the probability of beam of light interception based on the contact frequency between the laser radar beam of light and the tree. In summary, the specific process is divided into three steps: 

>  1. Determine whether there is a point from the 3D voxel model grid. The grid with a point is marked as 1, the grid without a point is marked as 0, and the grid without a point indicates the gap in the canopy. For details, please refer to: https://blog.csdn.net/dayuhaitang1/article/details/122794348. 

![avatar]( 61e98727c4ed4a30a89a7909b002dcee.png) 

>  2. To calculate the leaf area denstiy (LAD), the formula is as follows: 

![avatar]( ebea5dd2b6b046a586d30d510a77fa84.png) 

 ![avatar]( 210091c0dd61414bb2c9273400efbafc.png) 

![avatar]( 3040ca54076247cfa60e5825b8736363.png) 

>  3. Utilize the accumulated LAI in the vertical direction of the LAD. 

![avatar]( 6acd3ce3140c49e6ac6c58e553085542.png) 

#  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574016924
 ```  
Achieve the effect: 

![avatar]( bebf9a0db2204aadaef3e81e18c69397.png) 

#  III. Summary 

>  Because the three-dimensional voxel model is still constructed in the process of using VCP, there are still some problems in the determination of voxel size, but there are some studies in this area, and interested students can conduct in-depth learning. Note: In LiDAR360, 1.5 times the average spacing of point clouds is used as the side length of voxel. 

#  References 

>  [1]Derivation, Validation, and Sensitivity Analysis of Terrestrial Laser Scanning-Based Leaf Area Index 



--------------------------------------------------------------------------------

Because I was very interested in the concave bag recently, I found information and made the following note. 

#  I. Introduction 

>  In two dimensions. 

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

     The circle of alpha in a finite disordered set of points 

          S 

         S 

     Scroll in S, when 

          a 

         \alpha 

     When the value of α is large enough, the circle will not roll into the interior of the point set, then the points that the circle rolls through are connected to the point set 

          S 

         S 

     The boundary of S, the set of points 

          S 

         S 

     The concave package of S; when 

          a 

         \alpha 

     If the value of α is sufficiently small, then each point may be a boundary point, as shown in the figure below. 

![avatar]( 20200621142835761.png) 

#  Second, algorithm implementation 

##  2.1 Algorithm steps 

>  (1) Find the connection between any two points, with a total of N * (N-1)/2. (2) Assume that the radius of the ball is R, disconnect all connections with a distance greater than 2R, because it must be rolled in. (3) Make a circumscribed circle with a radius R for the two points of any remaining link, then there are at most two feasible solutions, and there is a third point in the circumscribed circle. It is considered invalid, and only the circumscribed circle does not contain any third point is retained; (4) The connections corresponding to all remaining circumscribed circles constitute boundary information. The above is only one of the basic algorithms. If you need to improve efficiency, you can achieve the goal by establishing a Delaunay triangular surface and checking symmetry. 

##  2.2 Code implementation (MATLAB) 

Here is a simple implementation method according to the idea, but the execution efficiency is not high, and the large amount of data becomes relatively slow. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574079075
 ```  
#  III. Achieving results 

![avatar]( 2020061709421886.png) 

#  IV. AlphaShape Algorithm in MATLAB 

Finally, using the alphaShape algorithm in MATLAB to calculate the area of the canopy point cloud projection, the effect is as follows, and the speed is very fast. 

>  AlphaShape.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574079075
 ```  
>  PointsAverageSpacing.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574079075
 ```  
![avatar]( 068686cdf53e4f62b1dbe6204cdade6e.png) 

 Achieve the effect:  

![avatar]( 961974df7fae4ad89ed9616ad1fed799.png) 



--------------------------------------------------------------------------------

#  I. Introduction 

>  I saw such a method for calculating the canopy volume from a certain paper (I can't remember the "_") before: 1. First, use the canopy adaptive slicing algorithm to merge and classify the slices of trees. For details, please read this blog: Canopy Adaptive Slicing Algorithm. 2. Then perform its volume value (AlphaShape) based on the merged slice layer. One advantage is that it can better remove some gaps in the canopy (of course, there may be other benefits, but I can't remember clearly). 3. Finally, add the volume value of each slice to calculate the volume value of the entire tree. 

#  Implementation code 

>  Graham.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574034446
 ```  
>  PolarAngle1.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574034446
 ```  
>  PointsAverageSpacing.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574034446
 ```  
>  AdaptiveSlicingV2.m 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574034446
 ```  
#  III. Achieving results 

>  Console output: 

![avatar]( 03d6c07d15b34f109d4600e5dbc4c859.png) 

>  Excel Sheet: 

![avatar]( 63b66c2ed1294105bdaa63e8f8a437e2.png) 

#  reference 

>  [1] Canopy adaptive slicing algorithm 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

