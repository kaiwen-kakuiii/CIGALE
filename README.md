# CIGALE-Configuration
CIGALE utlizes a fixed grid structure for model parameters. All the model parameters will only be computed once and stored in the memory (Thus it requires more memory than Prospector). Then it will use different parameter combinations to reconstruct model spectrum and calculate its corresponding Chi-square and probobality weight. The best-fit model is extracted from the likelihood distribution (not necessary the minimum Chi-square one).

Description:
  1. CIGALE_How_to is the official tutorial which I followed mostly.
  2. m87_new.vot is the input photometry file.
  3. pcigale.ini is the model configuration file.
  4. results.fits is the best run physical parameters.

Note:
   If you ran too many models (too many parameter combinations), your process may be killed in several seconds or you may encounter bus error (core dumped). All of these indicates you ran out of memory (physical memory). My suggestion is keep an eye on the KiB Swap (it is actually the space in your driver, not in memory), if its usage is rapidly increasing: you should increase physical memory OR use less model parameters. 
   For example, I ran CIGALE of 2e7 models with 12GB memory.
