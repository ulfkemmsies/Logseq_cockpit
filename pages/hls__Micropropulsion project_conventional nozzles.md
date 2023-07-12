file-path:: file://C:/Users/ulfkemmsies/Zotero/storage/ZGU9S2LZ/Micropropulsion project_conventional nozzles.pdf

- The thrust coefficient of the configuration can then be determined to be
  hl-page:: 3
  ls-type:: annotation
  id:: 6477784c-aac4-4c6e-8cd0-d2f4ad031bb1
  hl-color:: yellow
  \(C_F=\frac{F}{p_c \cdot A_t}\)
- # Performance Losses
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 6477799f-6d0c-471d-ba86-8709d9e9a69b
- he Reynolds number of the flow in a nozzle is a good measure for how large exactly this boundary layer is, and is traditionally given by
  hl-page:: 3
  ls-type:: annotation
  id:: 6477788d-df5f-41d6-b73e-dd86a32bc315
  hl-color:: yellow
  \(R e=\frac{\rho \cdot v \cdot D}{\mu}\)
- For micro-nozzles with a non-circular cross section, the diameter D can be replaced with the hydraulic diameter Dh using 
  hl-page:: 3
  ls-type:: annotation
  id:: 647778de-3273-47f5-804b-6585e9d4a8be
  hl-color:: yellow
  \(D_h=\frac{4 A}{p}\)
  Where A is the cross-sectional area, and p is the perimeter.
- smaller nozzles will naturally cause the flow Reynolds number to become very small. Where regular nozzles operate at Reynolds numbers well above 100,000, micro-nozzle Reynolds numbers can drop much lower than that.
  ls-type:: annotation
  hl-page:: 3
  hl-color:: red
  id:: 6477790c-5d40-42cc-9686-2d82b091d0bf
- ## Divergence Loss 
  hl-page:: 4
  ls-type:: annotation
  id:: 64777a4f-ee95-4084-b75a-a3e93bc8ce39
  hl-color:: yellow
  The first loss to reduce the performance of a nozzle is the divergence loss. Any nozzle that has an exit half angle larger than 0◦ will not eject gases parallel to the direction of thrust. The flow will have momentum components in directions perpendicular to the thrust vector. Because the nozzle is symmetric, these perpendicular momentum components cancel each other out and typically do not cause thrust misalignment. They do however contribute to a loss in thrust, as not all momentum is utilized to propel the spacecraft forward. The resulting loss is calculated as a factor, called the divergence thrust correction factor. It is given by 
  \(\epsilon_{d i v}=1-\frac{1-\cos (\alpha)}{2}\)
  Where α is the exit half angle of the nozzle. As can be seen, this loss factor is dependent only on the exit half angle, and affects large and small nozzles to a similar degree.
- ## Boundary Layer Losses
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 64777e7a-ea14-4eb4-911e-8c29665fb7e6
  hl-stamp:: 1685552765839
- Due to viscous flow effects, the flow travels at a slower speed close to the nozzle walls. This effectively "deflects" the full flow, and affects nozzle performance.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: red
  id:: 64777ef4-0e05-4c1b-839a-d05a3acfeb5c
- Boundary layer characterization is perhaps the most important element in predicting performance losses for micro-nozzles, as they significantly change the effective internal geometry. 
  ls-type:: annotation
  hl-page:: 4
  hl-color:: red
  id:: 64777f04-a807-4cae-9a9e-5e6945786813
- Low Reynolds number significantly increases the skin friction coefficient. This directly affects the effective flow deflection caused by the boundary layer. Low Reynolds numbers inherently cause boundary layers to grow larger.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: red
  id:: 64777f27-87a0-4f42-80b2-61b816162320
- According to flat plate boundary layer theory, the skin friction coefficient for incompressible, laminar flow is given by 
  hl-page:: 4
  ls-type:: annotation
  id:: 64777f30-ce0a-485d-ab59-5e6428ec805b
  hl-color:: yellow
  \(c_{f x}=\frac{0.664}{\sqrt{R e_x}}\)
  This equation explains why lower Reynolds numbers increase the skin friction coefficient.
- As a result of boundary layer growth, the effective nozzle areas are reduced.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: red
  id:: 64777f8b-695c-41a1-8b5e-8388a0144d4e
- Subsequently, the momentum thickness and displacement thickness are given by
  hl-page:: 4
  ls-type:: annotation
  id:: 6477811c-52bc-41f3-a2ed-79623b1acbe5
  hl-color:: yellow
  \(\begin{gathered}\theta_x=c_{f x} \cdot x \\ \delta^*=2.59036 \cdot \theta_x\end{gathered}\)
  The displacement thickness provides a measure for how much the flow is effectively "displaced" by the boundary layer.
- The true area ratio of a nozzle can then be found using
  hl-page:: 4
  ls-type:: annotation
  id:: 647781a7-8d55-4d7f-ae28-6de21123e3b1
  hl-color:: yellow
  \(\left(\frac{A_e}{A_l}\right)_{\text {true }}=\frac{2 \cdot\left(R_e-\delta^*\right)}{W_t}\)
  Where Wt is the throat width. It is important to note that here the throat diameter remains unchanged.
- The boundary layer is assumed to start developing at the throat, and increase in size until the nozzle exit.  Furthermore, this boundary layer solution assumes the flow remains laminar and attached. This assumption can be made for low Reynolds number flow, as the higher flow viscosity makes turbulent flow less likely.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: red
  id:: 647781bd-3510-43e5-8a8e-eeadafe0c6b2
- ## Momentum Losses 
  hl-page:: 5
  ls-type:: annotation
  id:: 647781eb-b1d5-486f-a520-19575caeb86e
  hl-color:: yellow
  In addition to the modification of effective nozzle geometry, the presence of a boundary layer also causes momentum losses. The flow loses momentum in the boundary layer, and this has to be seperately accounted for. The thrust loss due to momentum is given by
  \(\Delta F_{\text {momentum }}=\left(\rho_c \cdot u_c \cdot\left(2 \pi R_c\right) \cdot \theta_c\right) \cdot u_e\)
  Note that the circumference term here must be replaced with the equivalent perimeter for nozzles of non-circular cross section.
-
- # Reference Temperature Approach
  hl-page:: 5
  ls-type:: annotation
  id:: 648c66af-cffd-4606-8ac3-eced38495e20
  hl-color:: yellow
  The approach to predicting boundary layer properties presented in the previous section is based on the assumption that the flow is incompressible. However as the flow is accelerated through the nozzle, it becomes supersonic. This means it can no longer be assumed that the flow is incompressible. 
  The "Reference Temperature Approach", whereby the skin friction coefficient is corrected with a factor that is based on an average temperature across the boundary layer. Such a correction can be made using:
  \(c_f=c_{f, i}\left(\frac{T_w / T_0+1}{2}+0.22 \frac{\gamma-1}{2} M^2\right)^{-0.6}\)
  Where Tw is the wall temperature, and To is the stagnation temperature at the point where the skin friction coefficient is being determined. We consider only the exit stagnation temperature here, since the flat plate boundary layer characteristics will be determined at the exit of the nozzle to quantify the loss in exit area. The exit total temperature is determined using isentropic relations in the equation below. Note however that this equation could be used for any point along the nozzle, as long as the corresponding flow mach number is used:
  \(T_{0_e}=T_e \cdot\left(1+\frac{\gamma-1}{2} \cdot M_e^2\right)\)
- # Aggregate Performance Loss
  hl-page:: 5
  ls-type:: annotation
  id:: 648c6723-0de8-45da-9a0e-af3656ab5208
  hl-color:: yellow
  In order to determine the aggregate of all losses described in this chapter, a procedure for progressively implementing each loss must be determined. 
  The first step is to determine loss factors that are independent of boundary layer effects. The divergence thrust correction factor is thus first determined based on the divergent half angle. Next, the boundary layer properties are determined. The compressible skin friction coefficient, exit momentum thickness and exit displacement thickness are all calculated based on known flow parameters. 
  This allows the following steps to be taken in relation to boundary layer effects:
  1. Thrust reduction due to momentum loss is determined based on momentum thickness.
  2. The true area ratio is determined based on the displacement thickness.
  3. This true area ratio induces a lower exit pressure than predicted by IRT. The effective pressure ratio and exit pressures are iteratively determined using:
  \(\frac{\mathrm{A}_{\mathrm{e}}}{\mathrm{A}_{\mathrm{t}}}=\frac{\Gamma}{\sqrt{\frac{2 \gamma}{\gamma-1} \cdot\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)^{\left(\frac{2}{\gamma}\right)}\left(1-\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)^{\left(\frac{\gamma-1}{\gamma}\right)}\right)}}\)
  4. The resulting aggregate thrust loss is calculated. The aggregate thrust loss combines the divergence loss, momentum loss and reduced exit pressure. The true thrust, as estimated by this methodology, is thus given by:
  \(F_{\text {true }}=m \cdot \epsilon_{\text {div }} \cdot \sqrt{2 \cdot \frac{\gamma}{\gamma-1} \cdot \frac{\mathrm{R}_{\mathrm{A}}}{\mathrm{M}} \cdot \mathrm{T}_{\mathrm{c}} \cdot\left(1-\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)_{\text {true }}^{\frac{\gamma-1}{\gamma}}\right)}-\Delta F_{\text {momentum }}\)
  The thrust coefficient can then be determined with:
  \(C_{F_{\text {true }}}=\frac{F_{\text {true }}}{p_c \cdot A_t}\)