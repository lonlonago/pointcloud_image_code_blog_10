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

