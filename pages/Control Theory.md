- [[State Space]] Model
	- The state space of [[Linear Time-Invariant System]] is:
	  $$
	  \begin{aligned}
	  \dot{x} &=A x+B u \\
	  y &=C x+D u
	  \end{aligned}
	  $$
		- State vector \(\quad x=\left[x_1 \ldots x_n\right]^T \quad\)
		- Control (input) vector \(\quad u=\left[u_1 \ldots u_k\right]^T\)
		- State matrix \(\quad A(n \times n) \quad\)
		- Control (input) matrix \(B(n \times k)\)
		- Output vector \(\quad y=\left[y_1 \ldots y_n\right]^T \quad\)
		- Output matrix \(\quad C(m \times n)\)
		- Feedthrough matrix \(D(m \times k)\)
	- **State vector & matrix** are defined by physics, the **output vector** is by user
	- Applied in various control applications: [[Kalman filter]] , [[LQR Controller]] , robust, MPC
- Trajectory of Linear Systems
- Stability of Linear Systems
	- The internal stability of linear systems depends only on the free movement.
	  ![image.png](../assets/image_1663350678213_0.png)
	- The above classification can be generalized to higher order systems with the concept of [[Eigenvalue]]s of the state matrix \(A\).
		- ![image.png](../assets/image_1663350821950_0.png)
			- If **all** eigenvalues are in the left hand plane \(\rightarrow\) the system is **asymptotically stable**
			- If at least **one** eigenvalue is in the right hand plane \(\rightarrow\) the system is **unstable**.
			- If there are eigenvalues on the imaginary axis \(\rightarrow\) check multiplicity.
		- The position of the eigenvalues also determine the free movement.
			- More negative real parts of the eigenvalue correspond to more damping.
			- Higher magnitude imaginary parts of the eigenvalue correspond to a higher oscillation frequency.
			-
- [[Laplace Transform]]
	- {{embed [[Laplace Transform]]}}
- Transfer Function
- Poles
- Zeros
- Frequency Response
- Mass-spring-damper system
- Step Response
	- A step response test is a standard tool to investigate the properties of a controller.
	- Overshoot is an occurrence when the controller moves the actual value beyond the reference value.
	  ![image.png](../assets/image_1663667764676_0.png)
	- Steady-state error is the difference between the reference value and the actual value after the controller settles down.
	  ![image.png](../assets/image_1663667787423_0.png)
	- Instability is a condition when oscillations fail to decrease and/or are amplified with time.
	  ![image.png](../assets/image_1663667807483_0.png)
	- Rise time: time for the actual value to travel between \(10 \%\) and \(90 \%\) of the reference value.
	- Settling time: time between the step onset and the moment when the error between the reference and actual value falls and stays below some threshold (e.g., 5\% of the reference value).
	- Time constant: time until the actual value reaches \(1-1 / \mathrm{e} \approx 63.2 \%\) of the reference value.
- Bode Plot
- Control System Design
- Feedback Control
- Impedance Control
	- Modelled on a spring-mass-damper system
	- $$F_{\text {ext }}=K\left(x_\mu-x\right)+D\left(\dot{x}_\mu-\dot{x}\right)$$
	  $$\tau_{ext} = J^{T} F_{ext}$$
	  $$\tau = \tau_{dyn} + \tau_{ext}$$
	- For a critically damped system, use $D=2 \cdot 0.7 \cdot \sqrt{K}$
	-
- PID Controller
	- ![image.png](../assets/image_1663667654913_0.png)
	- PID controller consists of proportional, integral and derivative terms:
	  $$
	  \dot{x} \equiv K_p\left(x_r-x\right)+K_I \int\left(x_r-x\right) d t+K_D \frac{d\left(x_r-x\right)}{d t}
	  $$
	- The proportional term acts on the error between the actual and the reference value of the controlled variable.
	- The integral term eliminates a residual error of the proportional term in a steady state.
	- The derivative term can anticipate the changes and reduces overshoots.
	- PID Tuning
		- | Parameter increase | Rise time | Overshoot | Settling time | Steady-state error | Stability |
		  | :--- | :--- | :--- | :--- | :--- | :--- |
		  | $K_{p}$ | Decrease | Increase | Minor effect | Decrease | Degrade |
		  | $K_{I}$| Decrease | Increase | Increase | Eliminate | Degrade |
		  | $K_{D}$ | Minor effect | Decrease | Decrease | Minor effect | Improve |
		- Proportional Gain Effect
		- Integral Gain Effect
		- Derivative Gain Effect
		-
- [[LQR Controller]]
- MPC Concept
-