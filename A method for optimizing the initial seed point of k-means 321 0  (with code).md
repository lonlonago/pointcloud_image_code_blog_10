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

