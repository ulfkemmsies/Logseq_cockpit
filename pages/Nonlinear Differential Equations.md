tags:: class

- Textbook:
	- ![(Universitext) Ferdinand Verhulst (auth.) - Nonlinear Differential Equations and Dynamical Systems-Springer-Verlag Berlin Heidelberg (1996).pdf](../assets/(Universitext)_Ferdinand_Verhulst_(auth.)_-_Nonlinear_Differential_Equations_and_Dynamical_Systems-Springer-Verlag_Berlin_Heidelberg_(1996)_1663128212221_0.pdf)
	-
- Main topics
  heading:: true
	- Stability bifurcation points described by linearization
	  collapsed:: true
		- Linearization
			- Constant matrix
			- Time-dependent matrix
				- Floquet Theory
		- Methods beyond linearization
			- Blow-up technique
			- Zero-real-part eigenvalues: more equilibrium points
			- Morse Theorem (find if integrals exist)
			- Liouville Theorem
			- Lyapunov Function
			- Perturbation methods (multiple time scale)
		- Approximations of functions
			- Naive perturbation methods
			- Multiple scales perturbation methods
			- Poincaré-Lindstedt method (periodic)
			- Averaging method
			- Regular + Singular perturbation methods
			-
	- Chapter 2: Autonomous functions
		- Autonomous functions only depend on the dependent variable \(y^{\prime}=F(y)\)
		- Translation property
			- Suppose that we have a solution \(\phi(t)\) in the domain \(D \subset \mathbb{R}^n\), then \(\phi\left(t-t_0\right)\) with \(t_0\) a constant is also a solution.
		- Phase-space
			- The space in which we describe the behaviour of the variables \(x_1, \ldots, x_n\), parametrised by \(t\), is called phase-space.
			  ![image.png](../assets/image_1663353363479_0.png)
			- A point in phase-space with coordinates \(x_1(t), x_2(t), \ldots, x_n(t)\) for certain \(t\), is called a **phase-point**. In general, for increasing \(t\), a phase-point shall move through phase-space.
			-
		- Orbits
			- We shall use one of the components of \(x\), for instance \(x_1\), as a new independent variable; this requires that \(f_1(x) \neq 0\). With the chain rule we obtain \((n-1)\) equations:
			  $$
			  \begin{gathered}
			  \frac{d x_2}{d x_1}=\frac{f_2(x)}{f_1(x)} \\
			  \vdots \\
			  \vdots \\
			  \frac{d x_1}{d x_1}=\frac{f_n(x)}{f_1(x)}
			  \end{gathered}
			  $$
			  Solutions of the above system in phase space are called **orbits**.
			- If the existence and uniqueness theorem applies to the autonomous equation, it also applies to the above system, describing the behaviour of the orbits in phase-space. **This means that orbits in phase space will not intersect.**
				- It follows from the existence and uniqueness theorem that an equilibrium solution can never be reached in a finite time (if an equilibrium solution could be reached in a finite time, two solutions would intersect).
			- The arrows indicate the direction of the motion of the phase points with time; the motion of a set of phase points along the corresponding orbits is called the **phase flow**.
		- Critical Points
			- $$
			  f_1(a)=f_2(a)=\ldots=f_n(a)=0 .
			  $$
			  The point \(a \in \mathbb{R}^n\) is a zero of the vector function \(f(x)\) and we shall call it a critical point; sometimes it is called an equilibrium point.
			- A* critical point* is *isolated *if it is the only critical point in some small "neighborhood" of the point.
			- A critical point corresponds with an equilibrium solution (or stationary solution) of the equation: \(x(t)=a\) satisfies the equation for all time.
			- A critical point \(x=a\) of the equation \(\dot{x}=f(x)\) in \(\mathbb{R}^n\) is called a **positive attractor** if there exists a neighbourhood \(\Omega_a \subset \mathbb{R}^n\) of \(x=a\) such that \(x\left(t_0\right) \in \Omega_a\) implies \(\lim _{t \rightarrow \infty} x(t)=a\). If a critical point \(x=a\) has this property for \(t \rightarrow-\infty\), then \(x=a\) is called a **negative attractor**.
			- Types of critical points
				-
				- Centres are critical points where trajectories travel in closed elliptical orbits around the critical point.
				- Saddles are critical points where trajectories can be pulled in different directions from the point.
				  ![image.png](../assets/image_1663354879100_0.png)
				-
		- Linearization
			- To find attraction properties in the neighborhood of critical points $x = a$, linearize with the first term of a Taylor Series expansion.
			  \(\dot{x}=\frac{\partial f}{\partial x}(a)(x-a)+\) higher order terms.
			- A system is called *almost linear* (at a critical point (x0,y0)(x0,y0)) if the critical point is isolated and the [[Jacobian]] at the point is invertible, or equivalently if the linearized system has an isolated critical point.
		- Periodic Solutions
			- Suppose that \(x=\phi(t)\) is a solution of the equation \(\dot{x}=f(x), x \in D \subset \mathbb{R}^n\) and suppose there exists a positive number \(T\) such that \(\phi(t+T)=\phi(t)\) for all \(t \in \mathbb{R}\). Then \(\phi(t)\) is called a periodic solution of the equation with period \(T\).
				- If \(\phi(t)\) has period \(T\), than the solution has also period \(2 T, 3 T\), etc. Suppose \(T\) is the smallest period, than we call \(\phi(t) T\)-periodic.
			- A periodic solution of the autonomous equation \(\dot{x}=f(x)\) corresponds with a closed orbit (cycle) in phase-space and a closed orbit corresponds with a periodic solution.
			- Closed orbits of non-autonomous systems do not necessarily correspond with periodic solutions as the translation property no longer applies ($t$ is explicit on the RHS).
		- Orbital Derivative
			- Consider the differentiable function \(F: \mathbb{R}^n \rightarrow \mathbb{R}\) and the vector function \(x: \mathbb{R} \rightarrow\) \(\mathbb{R}^n\). The derivative \(L_t\) of the function \(F\) along the vector function \(x\), parameterised by \(t\), is
			  $$
			  L_t F=\frac{\partial F}{\partial x} \dot{x}=\frac{\partial F}{\partial x_1} \dot{x}_1+\frac{\partial F}{\partial x_2} \dot{x}_2+\cdots+\frac{\partial F}{\partial x_n} \dot{x}_n
			  $$
			  where \(x_1, \ldots, x_n\) are the components of $x$ . $L_t$ is called the orbital derivative.
		- First Integral
			- Consider the equation \(\dot{x}=f(x), x \in D \subset \mathbb{R}^n\); the function \(F(x)\) is called first integral of the equation if in \(D\) holds
			  $$
			  L_t F=0
			  $$
			  with respect to the vector function \(x(t)\), where $L_t$ is the orbital derivative.
			- First integrals are constant along a solution, and are also called constants of motion.
		- Integral Manifold
			- Taking a first integral F(x) = constant leads to a level set containing orbits of the equation. Such a level set consists of a family of orbits called an integral manifold.
		- Invariant Set
			- Consider the equation \(\dot{x}=f(x)\) in \(D \subset \mathbb{R}^n\). The set \(M \subset D\) is invariant if the solution \(x(t)\) with \(x(0) \in M\) is contained in \(M\) for \(-\infty<t<+\infty\). If this property is valid only for \(t \geq 0(t \leq 0)\) then \(M\) is called a positive (negative) invariant set.
		- Non-degenerate critical points
			- The critical point $x=a$ of $F(x)$ is called a non-degenerate critical point if the [[Hessian Matrix]] of $F(x)$ has determinant zero i.e. is invertible.
			  $$\left|\frac{\partial^2 F(a)}{\partial x^2}\right| \neq 0$$
				- The requirement of non-degeneracy we can interpret as the requirement that the vector function \(\partial F / \partial x\) has a "non-degenerate linearisation" in a neighbourhood of \(x=a\).
		- Diffeomorphism
			- Abbreviation for transformation which is one-to-one, unique, \(C^1\) and of which the inverse exists and is also \(C^1\)
		- Morse functions
			- If \(x=a\) is a non-degenerate critical point of the \(C^{\infty}\) function \(F(x)\), then \(F(x)\) is called a Morse-function in a neighbourhood of \(x=a\).
			- The behaviour of a Morse-function in a neighbourhood of the critical point \(x=a\) is determined by the quadratic part of the Taylor expansion of the function. Suppose that \(x=0\) is a non-degenerate critical point of the Morse-function \(F(x)\) with expansion
			  \(F(x)=F_0-c_1 x_1^2-c_2 x_2^2-\ldots-c_k x_k^2+c_{k+1} x_{k+1}^2+\ldots+c_n x_n^2+\) higher order terms with positive coefficients \(c_1, \ldots, c_n ; k\) is called the index of the critical point. There exists a transformation \(x \rightarrow y\) in a neighbourhood of the critical point such that \(F(x) \rightarrow G(y)\) where \(G(y)\) is a Morse-function with critical point \(x=0\), the same index \(k\), and apart from \(G(0)\) only quadratic terms.
			- Morse Lemma
				- Consider the \(C^{\infty}\) function \(F: \mathbb{R}^n \rightarrow \mathbb{R}\) with non-degenerate critical point \(x=0\), index \(k\). In a neighbourhood of \(x=0\) there exists a diffeomorphism which transforms \(F(x)\) to the form
				  $$
				  G(y)=G(0)-y_1^2-y_2^2-\ldots-y_k^2+y_{k+1}^2+\ldots+y_n^2
				  $$
		-