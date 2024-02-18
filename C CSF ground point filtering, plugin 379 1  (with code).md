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

