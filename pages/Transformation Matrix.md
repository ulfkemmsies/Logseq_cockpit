- ![image.png](../assets/image_1663349184047_0.png)
- A homogeneous transformation matrix is a way to describe a pose (i.e., both position and orientation).
- It is a 4-by-4 matrix that combines the rotation matrix and the position vector:
  $$
  \boldsymbol{T}=\left[\begin{array}{cccc}
  r 11 & r 12 & r 13 & x \\
  r 21 & r 22 & r 23 & y \\
  r 31 & r 32 & r 33 & z \\
  0 & 0 & 0 & 1
  \end{array}\right]
  $$
- Multiplication of several transformation matrices produces subsequent transformations between coordinate frames (e.g., useful in robots with multiple joints).