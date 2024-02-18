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

