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

