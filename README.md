**Code for computing spectral analyses as in [Raut et al. (2020) PNAS](https://www.pnas.org/content/117/34/20890)** 

**spectral_template.m** -- The main script for performing spectral analysis. Takes an input time series matrix and creates a Nx1 vector of "intrinsic timescales" for the N time series.     
**create_blocks.m** -- uses a temporal mask (e.g., indicating low-motion frames that should be included) of the time series to generate blocks of contiguous frames that meet the desired minimum block duration \
**lagged_cov.m** -- creates multivariate empirical cross-covariance functions (i.e., in units of the sampling interval) \
**acf_hwhm.m** -- estimates intrinsic timescale for each time series, computed as half of the full-width-at-half-maximum of the autocorrelation function (from lagged_cov.m) after spline fitting

**Please direct questions to ryanvraut@gmail.com**
