- ![image.png](../assets/image_1663349000886_0.png)
-
- 4D representation of space, one real number and three "imaginary" spatial dimensions
- In multiplication, quaternion on left is an action on a point (the quaternion on the right). Use the right hand to remember simultaneous moving and rotating of three axis circles.
- Unit quaternions give a simple way to encode the [[Axis-angle]] representation in four parameters
  $$
  \boldsymbol{q}=q_0+q_1 i+q_2 j+q_3 k
  $$
- Rotation in 3D by a quaternion corresponds to
  $$ r = q \cdot p \cdot q^{-1} $$
- Advantages: do not suffer from "gimbal lock", rotation around a single axis, more computationally efficient than rotation matrices
- Disadvantages: like with axis-angle there are nonunique solutions (two quaternions exist for the same rotation matrix), hard to imagine and visualise
- Note: like with [[Axis-angle]] , 3 rather than 4 independent parameters are sufficient to describe the unit quaternion.