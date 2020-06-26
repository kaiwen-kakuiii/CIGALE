# CIGALE-Configuration
Description:
  1. m87_new.vot is the input photometry file.
  2. pcigale.ini is the model configuration file.
  3. results.fits is the best run physical parameters.

Note:
  CIGALE utlizes a fixed grid structure for model parameters. All the model parameters will only be computed once and stored in the memory. Then it will use different parameter combinations to reconstruct model spectrum and calculate its corresponding Chi-square and probobality weight. The best-fit model is extracted from the likelihood distribution (not necessary the minimum Chi-square one). 
