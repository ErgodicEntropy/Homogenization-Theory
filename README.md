# HomogenizationTheory
This project is centered around the homogenization of the popular laminated and chessboard problems using FreeFem++ software program. A customized problem is discussed afterwards (reversed Turing pattern).\
Homogenization theory is the study of the process of homogenization in micromechanics and composite materials. Homogenization is the phenomenon of buffering variation and rendering the composite material homogeneous in terms of its properties by replacing it with a virtual equivalent homogenized copy of itself. In fact, the heterogeneity that is naturally present in composite materials make it harder for numerical simulation to perform computation on the system because of the amount of precision needed (at the level of the microstructure scale) to get accurate results, the computation then becomes exhaustive and expensive thus the use of homogenization techniques to alleviate the computational load.

## What is Homogeneity?


Homogeneity is the uniformity of a given property (electrical conductivity, elasticity, dielectric constant (Bruggeman's model)...etc) as a result of statistical average. Contrast to that, heterogeneity is when the percolation threshold is not reached. Examples of heterogeneity are the famous Turing patterns arising from the Turing instability (similar to Plateau-Rayleigh instability, Taylor-Rayleigh instability...etc) resulting from differential diffusion (different chemical species have different diffusion or self-diffusion coefficients)\
Homogeneity doesn't depend on the complexity of the system, meaning that all systems, regardless of their complexity (atoms, galaxies, humans..etc), exhibit homogeneity or heterogeneity. However, these notions are scale-dependent (what is homogeneous on the macroscopic level may be heterogeneous on the microscopic level). Homogeneity is a form of mixing which is a form of ergodicity, homogeneity doesn't conserve information but it abstracts it and encode it in a statistical average (usually harmonic mean as opposed to arithmetic mean)

## What is Homogenization?

From the point of view of set/relations theory, homogenization is an equivalence relation: it's reflexive, symmetrical and most importantly transitive. This last property of transitivity is the tenet of the second law of thermodynamics and moderation law as applied to intensive variables mixing (unlike extensive variables, intensive variables are emergent properties subject to moderation law eliminating their heterogeneity as ''perturbation'' thus they are naturally homogeneous; one could take the example of consciousness as an emergent phenomenon thus an intensive variables whilst society is the result of such moderation ie; societal laws are the results of interactionist homogenizations of individual consciousnesses).\
Formally speaking, homogenization is the process of replacing an equation (usually a partial differential equation) with highly oscillating coefficients (a(x/e)) with uniform homogenized coefficients (usually harmonic mean 1/<1/a>). But why? Remember, rescaling/scaling is a form of acceleration and deceleration, so basically what homogenization does is get rid of fast variable x/e (it's fast because of the small order of magnitude of e; microstructure scale) because it's computationally expensive to deal with extremely fast variations. To be more precise, it's not about ''speed'' really, we are not setting a timer and counting how fast the structure changes with time. Instead, it's about how steep the change is (say; norm of the gradient) when moving in the local neighborhood. In a sense, it's a form of condition number that captures how sensitive the structure is to change as a result of a tiny smooth change in spatial coordinates within their neighborhood (homogenization is thus the lowering of such a number down to zero).\
The intuition behind homogenization is known as effective medium approximation (one seen in continuum mechanics with the continuum hypothesis, in molecular dynamics with coarse-grained reduced representations..etc) which is a mean-field approach meaning that it performs some sort of dimensionality reduction (similar to machine learning's DR) of the material into lower dimension by averaging out details and encoding all statistical information in Representative Volume Element (RVE) while adding a perturbation parameter known as ''corrector'' that accounts for the loss of information, as discussed above, resulting from homogenization. Thus, homogenization theory is a special variant of perturbation theory in which the equations are perturbed from their homogeneous states by an estimate that reflects the information loss of the heterogeneous state.

## Future Considerations: 
1. Turing patterns
2. Voronoi Cell patterns
3. Founder effect
4. Crystallization effect
