Executive Summary:
- There are previous papers on QC for Plasma Dispersion Relations, but here we implement NISQ algorithms to small plasma setups
- We apply the Xie algorithm to find the complex eigenvalues of Plasma Instabilities
- We find that the Electron Weibel instability suffers a 2nd order phase-transition at the cut-off wavenumber. We provide an intuitive physical picture for this
- We compute several observables to "flag" and characterize unstable regions in the phase-diagram of these plasma setups
- We compare Fluid and Kinetic models
- For a toy-model, we manage to compute all results in closed-form


Outline:
- TSI fluid: 4x4 matrix
    - demo of branches (requires error bars from cloud of points around the local minima)
    - demo of entanglement entropy
- Weibel fluid: 10-moment 20x20 matrix ???
    - 2D (k,T) phase-diagram
    - possibly too expensive to run on current hardware
- Appendix: solved 2x2 matrix example
    - cost function, gradients
    - example runs on IBM QPUs (free-tier)

Dispersion Relation solvers:
        Fluid:
            Gkeyll https://gkeyll.readthedocs.io/en/latest/index.html#
        Kinetic:
            ALPS http://alps.space/
            PLUME https://github.com/kgklein/PLUME
