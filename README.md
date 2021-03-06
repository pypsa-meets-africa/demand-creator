# DEMAND-CREATOR

Status: Prototype
-----------------
A package to create electricity demand prediction for any arbitrary shape using ML

**Training data:**
- histortic and future hourly temperature time series
- histortic and future hourly humidity time series
- hourly wind speed
- yearly GDP
- ...

**General note:**
- Data should be available by default globally, in high resolution rasters (.nc format), over 30+year
- Methods should be written that more accurate local data can be integrated
- Methods should allow to modify flexibly climate change impacts on the demand

**Possible future?** Create demand timeseries for other sectors such as heat demand, industrial demand and transportation demand


--------------------------------
**Snakemake exercise**

- Install pypsa-africa or pypsa-eur as conda environment, see [here](https://github.com/pypsa-meets-africa/pypsa-africa#installation)
- Run the following to get an output

```
conda activate pypsa-africa

snakemake --cores 1 salt_bae_extractor
```
- Try to understand how this output was generated in the Snakefile
- Analyse the python scripts
- Play around with the config.yaml
