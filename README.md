# let's learn about some tilty spinny bois

Welcome to the public repository for calculating some key dynamical quantities for M dwarf planets excited into Cassini state 2. 


# get started

  * download `tutorial.ipynb`
  * download supporting files:
    * Kepler sample: `koi_mdwarf_multis_planets.fits`
    * Not-Kepler sample: `other_struct_planets_extra_teq.fits`
    * Lookup table of Gaia magnitudes for Not-Kepler planets:`non_kepler_candidates_gaia_mag.txt` (Gaia mag is comparable to Kepler mag)
  * screech 

If you're feeling ✨adventurous✨, you can see what's going on in `wobblebaby_withBeta.ipynb`. This is the notebook for calculating how the transit duration for each planet in the sample will change as the orbit precesses (and the chord of the transit moves around on the disk of the star and changes length). _It is very much a working notebook_ (with a lot of deprecated/old code the farther down in the notebook you go). 

For starters, you will need to change the paths for saving figures and text files. 

Also, I haven't uploaded all the supporting files to make it work, namely the MCMC posteriors for $\sigma T_{dur}$, the observing uncertainty for a present-day observation using a ground-based 10m-class telescope. If you really want to run it, just hardcode `obs_tdur_err = Tdur_err`. This will change what the observability threshold is for the planet to be the observation uncertainty for the observation at the discover epoch (ex. Kepler uncertainties are typically 2 minutes, so you won't be able to detect any changes in transit duration shorter than two minutes).

# relevant reading

[_Plausibility of Capture into High-obliquity States for Exoplanets in the M Dwarf Habitable Zone_, Guerrero, Ballard, and Su](https://ui.adsabs.harvard.edu/abs/2024ApJ...975..256G/abstract)




