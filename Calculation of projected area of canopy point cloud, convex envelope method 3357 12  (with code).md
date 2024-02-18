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

