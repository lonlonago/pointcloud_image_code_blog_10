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

