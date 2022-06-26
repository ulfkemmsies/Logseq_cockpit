- In the probabilistic modelling of life-cycle management, the [[Renewal Theorem]] plays a key role in the computation of the expected number of renewals and the cost rate associated with a management strategy.
  hl-page:: 1
  ls-type:: annotation
  id:: 621b9736-4ba1-441b-93dc-74a672d313e1
- To minimise the risk associated with failure of an infrastructure system, inspection and replacements are routinely carried out. Because of uncertainty associated with degradation mechanisms, operational loads and limited inspection data, probabilistic methods play a key role in developing cost effective management models
  hl-page:: 1
  ls-type:: annotation
  id:: 621b97e1-c50b-4668-b36e-d25537482dbe
- The theory of [[Stochastic Renewal Processes]] and the renewal theorem have been fundamental to the development of risk-based asset management models
  hl-page:: 1
  ls-type:: annotation
  id:: 621b980e-7ab4-4554-b6ed-43ad0eec0599
- For sake of conceptual simplicity, we consider a discrete time scale to model the process of times at which failure occurs with an independent, identically distributed (iid) sequence of 0–1 random variables, where 1 means occurrence of failure. This leads to a discrete version of the [[Poisson process]] where the times between failures are independent, geometrically distributed random variables.
  hl-page:: 1
  ls-type:: annotation
  id:: 621b9c45-ea0f-46b0-ad48-974303b1cd00
- However, in cases where the geometric distribution of the inter-occurrence time cannot be justified, a natural way to generalise the analysis is to model it as a renewal process.
  hl-page:: 1
  ls-type:: annotation
  id:: 621b9c5f-408f-4c23-9141-83df72bb62b9
- The basic premise is that the lifetime ($T$) of a component is a random variable
  hl-page:: 2
  ls-type:: annotation
  id:: 621b9ed3-ac8c-446e-8341-a2273cfa8c00
- The probability distribution of $T$ is given as $\mathbb{P}(T=k)=p_{k} \quad(k=1,2, \ldots)$
  hl-page:: 2
  ls-type:: annotation
  id:: 621b9efd-960d-48e8-9099-8bcb2ce0ed81
- The probability generating function of ($p_k$) is given by $P(z)=\sum_{k=0}^{\infty} p_{k} z^{k}$ where $p_0 = 0$
  hl-page:: 2
  ls-type:: annotation
  id:: 621b9f68-44ee-403f-9dfb-35006d939460
- The probability distribution ($p_k$) is referred to as the **renewal distribution**
  hl-page:: 2
  ls-type:: annotation
  id:: 621b9fa1-cebb-4e7c-8ec5-81c820a1dcb9
- The expected number of renewals up to timet(firstmoment) is referred to as the renewal function, i.e.,M(t)=E(Nt).
  ls-type:: annotation
  hl-page:: 3
  id:: 621bafa7-f368-4e38-87f6-b042c3d23fe0
- The following recursion can be used to calculate the sequence as $u_{n}=\sum_{k=1}^{n} p_{k} u_{n-k} \quad\left(n \geq 1, u_{0}=1\right)$
  hl-page:: 3
  ls-type:: annotation
  id:: 621bb0b3-8b3d-47db-b023-3377f91c333c
	- This is an approximation of the convolution integral in [[../assets/Bednara_thesis_2008_-_Methds_for_approximating_the_availability_functions_1645798062058_0.pdf]]
- So, the basic idea is that the renewal rate can be directlyobtained from the generating function of the renewaldistribution. Then, it can be used to compute momentsof the number of renewals.
  ls-type:: annotation
  hl-page:: 4
  id:: 6229c7f5-d796-4ac1-ad1c-e92e0c35f62e