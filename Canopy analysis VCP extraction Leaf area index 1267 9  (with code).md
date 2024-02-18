#  I. Introduction 

>  This method was first proposed by Omasa et al. to calculate the probability of beam of light interception based on the contact frequency between the laser radar beam of light and the tree. In summary, the specific process is divided into three steps: 

>  1. Determine whether there is a point from the 3D voxel model grid. The grid with a point is marked as 1, the grid without a point is marked as 0, and the grid without a point indicates the gap in the canopy. For details, please refer to: https://blog.csdn.net/dayuhaitang1/article/details/122794348. 

![avatar]( 61e98727c4ed4a30a89a7909b002dcee.png) 

>  2. To calculate the leaf area denstiy (LAD), the formula is as follows: 

![avatar]( ebea5dd2b6b046a586d30d510a77fa84.png) 

 ![avatar]( 210091c0dd61414bb2c9273400efbafc.png) 

![avatar]( 3040ca54076247cfa60e5825b8736363.png) 

>  3. Utilize the accumulated LAI in the vertical direction of the LAD. 

![avatar]( 6acd3ce3140c49e6ac6c58e553085542.png) 

#  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574016924
 ```  
Achieve the effect: 

![avatar]( bebf9a0db2204aadaef3e81e18c69397.png) 

#  III. Summary 

>  Because the three-dimensional voxel model is still constructed in the process of using VCP, there are still some problems in the determination of voxel size, but there are some studies in this area, and interested students can conduct in-depth learning. Note: In LiDAR360, 1.5 times the average spacing of point clouds is used as the side length of voxel. 

#  References 

>  [1]Derivation, Validation, and Sensitivity Analysis of Terrestrial Laser Scanning-Based Leaf Area Index 

