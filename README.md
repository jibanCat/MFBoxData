# MFBoxData
Simulation data from *MF-Box: Multi-fidelity and multi-scale emulation for the matter power spectrum* (in prep).

Data here include matter power spectra from dark-matter only N-body simulations with different fidelities and boxsizes:

- Format of naming: `dmo_{number of simulations}_res{particle load}box{box size}`
- For example, `dmo_24_res512box256`: 24 simulations in 512^3 particle load and 256 Mpc/h box.

## Parameters

In the `cc_emulator_powerspecs.h5` file:
| Parameter | Explanation |
| --- | --- |
| `bounds` | maximum and minimum limits of the prior volume|
| `hubble` | Hubble parameter, h, which is H0 / (100 km/s/Mpc)|
| `kfmpc`  | k bins of power spectra in h/Mpc |
| `modes`  | number of modes in a given power spectrum bin |
| `ns` | Scalar spectral index |
| `omega0` | Total matter density at z=0 (includes massive neutrinos and baryons) |
| `omegab` | Baryon density|
| `parameter_names` | String names of parameters |
| `params` | Latin-hypercube samples of parameters |
| `powerspecs` | Matter power spectra |
| `scalar_amp` | A_s at k = 0.05, comparable to the Planck value.
| `scale_factors` | Scale factor, 1 / (1 + redshift) |
| `zout` | The redshifts of the simulations |

