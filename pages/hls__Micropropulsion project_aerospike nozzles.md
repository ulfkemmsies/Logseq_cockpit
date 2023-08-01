file-path:: file://C:/Users/ulfkemmsies/Zotero/storage/WMQRQSZP/Micropropulsion project_aerospike nozzles.pdf

- Micronozzles are know for having low performance and efficiency under low Reynolds number (usually under 1000). This is usually attributed to the effect of viscous forces. To study the performance of nozzles, performance parameters are used. For this study, three performance parameters where chosen: thrust efficiency \(\eta_F\), discharge coefficient \(C_D\), and specific impulse efficiency \(\eta_{I_{s p}}\). They are defined as follows [6]:
  ls-type:: annotation
  hl-page:: 10
  hl-color:: yellow
  $$
  \begin{aligned}
  & \eta_F=\frac{F_{\text {meas }}}{F_{1 D}} \\
  & C_D=\frac{\dot{m}_{\text {meas }}}{\dot{m}_{1 D}} \\
  & \eta_{I_{s p}}=\frac{I_{s p_{\text {meas }}}}{I_{s p_{1 D}}}
  \end{aligned}
  $$
  The theoretical values are represented by the subscript \(1 D\) and are calculated through the principles of Ideal Rocket Theory as follows:
  $$
  \begin{gathered}
  \left.F_{1 D}=C_F p_c A_t=p_c A_t \sqrt{\frac{2 \gamma^2}{\gamma-1}\left(\frac{2}{\gamma+1}\right)^{\frac{\gamma+1}{\gamma-1}}\left(1-\frac{p_e}{p_c}\right.}\right)+A_e\left(p_e-p_{\infty}\right) \\
  \dot{m}_{1 D}=\frac{p_c A_t}{c^*}=\frac{\sqrt{\gamma}\left(\frac{2}{\gamma+1}\right)^{\frac{\gamma+1}{2(\gamma-1) p_c A_t}}}{\sqrt{R T_c}} \\
  I_{s p_{1 D}}=\frac{F_{1 D}}{\dot{m}_{1 D} \cdot g_0}
  \end{gathered}
  $$
	- \(I_{s p_{\text {meas }}}=\frac{F_{\text {meas }}}{\dot{m}_{\text {meas }} \cdot g_0}\)
	  hl-page:: 11
	  ls-type:: annotation
	  id:: 64c8b78f-ccd1-47a3-bf73-483e9093daa1
	  hl-color:: yellow
- [:span]
  ls-type:: annotation
  hl-page:: 13
  hl-color:: yellow
  id:: 648c778c-29f7-4263-854c-4af7e520abd0
  hl-type:: area
  hl-stamp:: 1686927243640
- ## Momentum Loss 
  hl-page:: 14
  ls-type:: annotation
  id:: 648c77b1-c0ef-4f95-8238-f6131af12217
  hl-color:: yellow
  The skin friction in the walls of a nozzle cause an effect that reduces the thrust of the propulsion system [17]. This parameter is named “momentum loss thickness” and can be represented to a force that has an axial component in the direction of thrust. By subtracting this amount from the thrust, it is possible to calculate the “measured” thrust and therefore the thrust efficiency
  \(\Delta F=\left(\rho_e \cdot u_e \cdot 2 \pi R_e \cdot \theta_e\right) \cdot u_e\)
- ## Effect of Viscous Forces 
  hl-page:: 19
  ls-type:: annotation
  id:: 648c77fe-0332-47ea-9dbb-93854b32f904
  hl-color:: yellow
  Another approach that can be taken to calculate the“experimental” value of thrust is using the relation derived by Spisz (1965) [13]. This expression is used to estimate the effect of the viscous forces caused by the boundary layer on the nozzle quality
  \(C_F=C_{F, i}-C_{F, v i s c}\)
  \(C_{F, v i s c}=\frac{17.6 e^{\frac{0.0032 A_e}{A_t}}}{\sqrt{0.773 R e_t}} \quad 2000 \leq R e_t \leq 10000\)
   Where \(C_F\) is the thrust coefficient corrected for viscous effects, \(C_{F, i}\) is the ideal thrust coefficient, and \(C_{F, v i s c}\) is the effect of the boundary layer on the thrust coefficient.
  \(C_{F, i}=\frac{F_{1 D}}{p_c \cdot A_t}\)
- To calculate the thrust efficiency, the following expressions were used:
  hl-page:: 20
  ls-type:: annotation
  id:: 648c780e-b115-4f27-9f12-fabfefb4df54
  hl-color:: yellow
  \(F_{\text {meas }}=C_F \cdot p_c \cdot A_t\)
  \(\eta_F=\frac{F_{\text {meas }}}{F_{1 D}}=\frac{C_F \cdot p_c \cdot A_t}{C_{F, i} \cdot p_c \cdot A_t}=\frac{C_F}{C_{F, i}}\)
- ## Discharge Coefficient 
  hl-page:: 23
  ls-type:: annotation
  id:: 64916422-68b3-4071-afd9-4f27beffde57
  hl-color:: yellow
  In Tang and Fenn (1978) an expression was derived to calculate the discharge coefficient that takes in consideration the effect of the boundary layer in reducing the effective nozzle throat area. In particular these effects are more significant for throat Reynolds number under 100000 . The expression was derived for choked axisymmetric nozzles with a circular cross-section [15]. The equation derived by Tang and Fenn reads as follows:
  $$
  C_D=1-\left(\frac{\gamma+1}{2}\right)^{3 / 4}\left(\frac{-2.128}{\gamma+1}+3.266\right) R^{-0.5}+9.428 \frac{(\gamma-1)(\gamma+2)}{(\gamma+1)^{0.5}} R^{-1}
  $$
  Where \(R\) is the modified throat Reynolds number that can be calculated through the expression [17]:
  $$
  R=R e_t\left(\frac{R^*}{R_t}\right)
  $$
  Where \(R^*\) is the radius of the throat and \(R_t\) is the throat radius curvature. From table 3.1 it is possible to retrieve the values for \(R^*\) and \(R_t\) :
  $$
  \begin{gathered}
  R^*=W_t=45 \mu \mathrm{m} \\
  \frac{2 R_t}{W_t}=10 \Leftrightarrow R_t=\frac{10 \cdot W_t}{2}=225 \mu \mathrm{m}
  \end{gathered}
  $$
  And with these values the discharge coefficient can be calculated for the different Reynolds numbers. The value of the specific heat ratio \(\gamma\) is 1.4 for nitrogen [5].
- The expression by Tang and Fenn (1978) was derived for adiabatic flow, in particular cold gases, flowing through smooth circular nozzles
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 64ae3eb1-af0e-4bdc-affd-a4ab94d5359b
- ## Effective vs. Geometric Area Ratio 
  hl-page:: 27
  ls-type:: annotation
  id:: 6491680c-df39-4514-9025-f748f4864751
  hl-color:: yellow
  In Bayt (1999) different micronozzles and their performance are studied. In particular, one of the studied designs is a micronozzle with a rectangular throat section and an area ratio of 16.9. The performance of this nozzle is studied for Reynolds numbers ranging from 382 to3721. Part of the research done in Bayt (1999) included the study of effective vs. geometric area ratio of the micronozzle for different Reynolds number.
- The data points obtained using the WebPlotDigitizer for effective and geometric area ratio are displayed in table 4.15. Additionally, the ratio between the two values is also shown. Table 4.15: Values of effective and geometric area ratio 
  hl-page:: 28
  ls-type:: annotation
  id:: 648c76ef-cc0e-4b0f-9bf7-81ff25fb2c7b
  hl-color:: yellow
  | Reynolds Number | Effective Area Ratio | Geometric Area Ratio | Efficiency |
  | :--- | :--- | :--- | :--- |
  | 382 | 10.147 | 16.9043 | 0.600 |
  | 574 | 11.078 | 16.8116 | 0.659 |
  | 1340 | 12.672 | 16.8812 | 0.751 |
  | 2488 | 13.689 | 16.8928 | 0.810 |
  | 3721 | 13.983 | 16.8 | 0.832 |
   The value of discharge coefficient was assumed to be the ratio between effective area ratio and geometric area ratio as it can be confirmed by equation 4.26. The values were plotted in figure 4.18.
  \(C_D=\frac{\dot{m}_{\text {meas }}}{\dot{m}_{1 D}}=\frac{\rho u A_{e f f}}{\rho u A_{g e o}}=\frac{A_{e f f}}{A_{g e o}}\)
- This function finds the best fit for the given values (which in this case are the values of the ratio between effective and geometric area ratio) and displays the equation for that fit, which in this case was a non-linear regression. For these values the relation found was equation 4.27.
  hl-page:: 29
  ls-type:: annotation
  hl-color:: yellow
  \(\frac{A_{\text {eff }}}{A_{\text {geo }}}=0.322135-\frac{38.6498}{R e}+0.063732 \cdot \log (R e)\)