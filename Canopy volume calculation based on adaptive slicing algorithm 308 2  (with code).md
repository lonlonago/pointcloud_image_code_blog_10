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

