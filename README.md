# X_to_GFF_tests

The final goal is to extract GFFs from cross sections. As the first step, we test on Compton Form Factors instead of the cross section.
For the vector CFFs (from GPDs $H^q$ and $E^q$):

$$\mathcal{H}(\xi, t) = \sum_q e_q^2 \int_{-1}^1 dx \, H^q(x, \xi, t) \left[ \frac{1}{x - \xi + i\epsilon} - \frac{1}{x + \xi - i\epsilon} \right],$$

$$\mathcal{E}(\xi, t) = \sum_q e_q^2 \int_{-1}^1 dx \, E^q(x, \xi, t) \left[ \frac{1}{x - \xi + i\epsilon} - \frac{1}{x + \xi - i\epsilon} \right].$$

and the corresponding GFFs are, 

$$A_{g}(\xi,t) = \int_{0}^{1} dx \, H_g^{DD}(x,\xi,t)$$ 

$$D_{g}(\xi,t) = \frac{1}{\xi^2} \int_{0}^{1} dx \, |\xi| \cdot D_g(x,\xi,t)$$

where we have,

$$
H_g(x,\xi,t) = H_g^{DD}(x,\xi,t) + |\xi| \cdot D_g(x,\xi,t)
$$

$$
E_g(x,\xi,t) = -|\xi| \cdot D_g(x,\xi,t)
$$


## Compton Form Factors to GFF

1, *Images lives on 2-d lattice*: Both $\mathcal{H}/\mathcal{E}(\xi, t)$, and $A/D_{g}(\xi,t)$ lives on the $\xi-t$ lattice, where $\xi$ is a function of energy. 

2, *Mask for missing value*: we should be able to handle missing value in some part of the phase space on the Compton Form Factor side but GFFs has no missing value because they are entirely from reconstruction.
