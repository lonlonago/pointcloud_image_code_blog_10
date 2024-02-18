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

