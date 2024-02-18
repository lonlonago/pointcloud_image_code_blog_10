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

