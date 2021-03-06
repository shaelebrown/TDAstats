# TDAstats (development version)

## Changes

* `calculate_homology` now accepts any variable storing a distance matrix as long as it can be coerced to a matrix

## Additions

* added option for `calculate_homology` to return a data frame instead of a matrix
* more code coverage
* added support for flat persistence diagrams (`flat = TRUE` in `plot_persist`)

# TDAstats 0.4.0

## Bug Fixes

* previous vignettes did not have citations and references section working properly; this has been fixed

## Changes

* added `standardize` parameter to `calculate_homology` and functionality to standardize point cloud size
* added `limit.num` parameter to `phom.dist` and functionality to consider only "significant" topological features

## Additions

* code coverage has been increased
* added support for distance matrix format for calculate_homology
* vignette has been added showing use of new distance matrix format
* `phom.dist` function to compare persistent homology of two point clouds/matrices

# TDAstats 0.3.0

## Bug fixes

* fixed bug in `plot_persist` where setting a shorter axis limit would cause the reference diagonal to disappear (thank you, @corybrunson)

## Changes

* changing size of `plot_persist` output figures still preserves one-to-one length ratio of horizontal and vertical axes (fixed coordinate system; thank you, @corybrunson)

# TDAstats 0.2.0

## Bug fixes

* fixed bug in `permutation_test` function that resulted in NAs in output
* fixed naming clash with `index_t` in C++ code; should make TDAstats compatible with Solaris systems

## Changes

* added `dim` parameter to `permutation_test` function to allow users to select maximum dimension for homology comparison

## Additions

* added automated testing using `testthat` package
* 4 sample datasets for users to learn/test TDAstats (and probably to follow future vignettes): unif2d, unif3d, circle2d, sphere3d
* added 2 vignettes introducing features of TDAstats to user through text and a case study

# TDAstats 0.1.0

* This is the first release of TDAstats.
