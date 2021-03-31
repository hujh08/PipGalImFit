Pipline for galaxy image fitting

# Introduction
This project aims to develop a pipline of galaxy image fitting, e.g. bulge/disk decomposition. Many useful facilities are designed for this purpose.

# Organization of data in directory and optional help files
For an observation, it corresponds to a directory, named by `root`. This top directory is kept as clean as possible, and subdirectories are created for all the fussy subsequent procedures, including intermediate data, for example analysis of sextractor, galfit for different models and so on. Following this guide, directory `root` only stores initial raw data and some basic results, e.g. sigma fits, mask of foreground and background, psf, et al.

To facilliate future work, maybe after very very long time, some help files are recommanded to record intermediate results and the meaning of data files in `root` and subdirectories. And these records are also helpful to develop automate routines. A main help file, with name `data.info` by default, stores the information of the data, like file name of data, region of target object and so on.

# Fitting Steps

## SIMD-like pipline
A pipline for a galaxy photometry measurement could be developed by two parts, the outer iteration, to walk along `root` of different observations, e.g. different galaxies and different bands, and the inner routine, that is work to the single observation. This running mode, in some kind, looks like the SIMD (Single Instruction, Multiple data) parallelism. Pipline here could be organized in a similar way as SIMD.

## Outer iteration

## Inner routine

### initiation of `root`

### preliminary analysis
Mainly analysis by `Sextractor`

### create galfit.00 from previous results

### strategies to run galfit

### collection of final result

# Visual Check

# Log System
