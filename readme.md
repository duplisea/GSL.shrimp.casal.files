# Report: Assessing rebuilding potential for Gulf of St. Lawrence shrimp stocks, *Pandalus borealis*, in the critical zone

**Authors:** Sophie Mormede, Daniel Duplisea, Marie-Julie Roux, Hugo Bourdages  
**Date:** December 2024  
**Contact:** Sophie Mormede [sofishconsulting@gmail.com](mailto:sofishconsulting@gmail.com)

## Description

These are the Casal2 inputs (.csl2) and main output files for the base case models.

- `estimate.log` contains the MPD outputs.
- `objectives.x` and `samples.x` contain the main MCMC outputs, one file per MCMC chain.

The final MCMC outputs of all quantities are excluded due to the size of the files.

## Recreating Final MCMC Outputs

To recreate the final MCMC outputs using the Casal2 software, run the following commands in the folder where `objectives.x` are located:

```bash
casal2 -c config-tab.csl2 -r -i samples.1 -t > quantities.1
casal2 -c config-tab.csl2 -r -i samples.2 -t > quantities.2
casal2 -c config-tab.csl2 -r -i samples.3 -t > quantities.3
```

## Software and Tools

A version of Casal2 is available at [https://github.com/alistairdunn1/CASAL2](https://github.com/alistairdunn1/CASAL2).

R extractor functions for Casal2 outputs are also provided on the above GitHub page.
