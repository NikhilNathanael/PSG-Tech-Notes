#FluidMechanics #DifferentialMomentEquations #Navier-StokesEquation
Let $dV$ be a small fluid element in a fluid.
	$\sigma_{nn}$ is the normal stress on a plane 
	$\tau_{nm}$ is the torsional stress on a plane in the $n$ direction acting towards $m$

The elementary edge forces acting along $x-\text{direction}$ is given by 
$$\begin{align*}
dF_s&=((\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x})dy dz-(\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x})) \\
 &+ (\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x})dy dz-(\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x}) \\
&+ (\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x})dy dz-(\sigma_{xx} + \frac{\delta \sigma_{xx}}{\delta x}) 
\end{align*}
$$
$$\begin{align*}
dF_s&=((σ_xx+(δσ_xx)/δx  dx/2)dy dz−(σ_xx  (δσ_xx)/δx  dx/2)dy dz)\\&+((τ_yx+(δτ_yx)/δy  dy/2)dx dz−(τ_yx−(δτ_yx)/δy  dy/2)dx dz)\\&+((τ_zx+(δτ_yx)/δz  dz/2)dx dy−(τ_zx−(δτ_zx)/δy  dz/2)dx dy)
\end{align*}$$