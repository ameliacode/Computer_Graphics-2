## Exercises

#### 1. Note: You can select any start position as you like, as long as it is in CCW.

|vertex array | index array |
|---|---|
| p | 0 |
| q | 1 |
| r | 2 |
| s | 0 |
|   | 3 |
|   | 1 |  

  
#### 2. Note: You can select any start position as you like, as long as it is in CCW.

|vertex array |  index array |
|---|---|
| (0,0,0) | 0 |
| (1,0,0) | 1 |
| (0,1,0) | 2 |
| (0,0,1) | 3 |
|         | 0 |
|         | 2 |
|         | 3 |
|         | 1 |
|         | 0 |
|         | 3 |
|         | 1 |
|         | 2 |  

#### 3. consequently, 24, 6, 24

#### 4. 614   
   Solution) Think of it in this way, we all know that a whole circle's angle is total 360 degrees, divide this in every 10 degrees results in 36 sided polygon by its latitude. With the 36 sided polygon, by longtitude, this polygon will be stacked upto 17 layers. (180 degrees divided by 10, however we have to exclude top and bottom, results in 17 layers in total → think as two hemispheres each by each).   
   Add these up, you'll get 612 + (top and bottom vertex) = 614   
   
   <p align="center"><img src="./img.PNG"></p>
   It actually is 614 vertices total.

#### 5.
|vertex array |  index array |
|---|---|
| (0,0,0) | 0 |
| (1,0,0) | 2 |
| (0,1,0) | 1 |
| (0,0,1) | 0 |
|         | 1 |
|         | 3 |
|         | 3 |
|         | 2 |
|         | 0 |
|         | 3 |
|         | 2 |
|         | 1 |  


#### 6. Following formula in page 18,  
   
   1) by Euler's polyhedron formula asserts:
   
   $$ v - e + f = 2 $$

   $$ 2e = 3f $$

   In a closed triangle mesh, every edge is shared by two faces, and every face has three edges. Derived from the equations above, we can know that the number of faces converges to twice the number of vertices.
