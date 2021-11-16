# [MagMet](http://magmet.ca)
This repository is for a brief description of MagMet.

Nuclear Magnetic Resonance spectroscopy is a powerful technique and is used widely for metabolomics studies. However, spectra analysis and manual spectral profiling to extract metabolite concentration is a time-consuming process and done by highly qualified personnel.  
To overcome these challenges, MagMet is developed.  

  The automatic NMR data analysis by MagMet is a two step process.  
1. NMR raw data processing
2. Profiling of the processed data

## [MagMet](http://magmet.ca) NMR data processing
MagMet reads raw data from Bruker and Varian instrumets using NMRglue.

  Then MagMet performs all the standard processing steps such as zero filling, Fourier transform, automatic phase correction, automatic baseline correction, and line-broadening. Finally, the processed spectrum is exported as CSV and JSON format for profiling.
  
  Some of the above steps are adopted from BAYESIL and optimized for a more robust result.

## [MagMet](http://magmet.ca) metabolomic profiling
MagMet uses a set of spectra of reference compounds as a library and searches them in biofluids by identifying the individual peak patterns. A complete novel algorithm is developed in-house for the detection process.

  After the detection process, it calculates the concentration of metabolites by regression analysis.  
Extensive testing has shown that the detection procedure is ~95% accurate and provides the concentration of metabolites within ~10% error of actual value.

  The current version of MagMet is optimized and validated for biofluids such as serum/plasma, fecal water.  
In addition, the optimization is in progress for the profiling of wine and beer.

Because of its completely automated workflow, MagMet can save thousands of dollars for lab and hundreds of working hours of trained employees’ time. The results will be consistent and batch effect will be minimum which is necessary for biomarker detection.



