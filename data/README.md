VLT/VISIR Calibrated Data

In these subdirectories you will find calibrated versions of data files used in
our publications.  In general, for each wavelength, you will find:

* A `.fits.gz` file that contains the original image, calibrated to units of
ergs/s/cm2/sr/um.  Sometimes these images have been destribed and filtered, and
sometimes the negative "B" beam has been removed to make a cleaner image.  We
only include the version of the data used in our papers.

* A `.fits.cmap.gz` file that is a cylindrically-mapped version of the image,
with planetocentric latitudes (-90 to 90) and System III West Longitude.  The
units are the same as those given above.  Note that these are usually converted
to brightness temperatures for plotting purposes.

* A `.fits.mu.gz` file that contains the emission angles for each pixel in the
original image.

* And sometimes, a `.fits.mu0.gz` file that contains the solar incidence angles
for each pixel in the original image.


The filenames proivide the time of the observation and the wavelength via the
following codes:  

* M-Band (5 micron) - sensing deep cloud opacity.

* J7.9 (7.9 micron) - sending stratospheric temperature near 10-20 mbar via
methane emission.

* PAH1 (8.6 micron) - sensing aerosol opacity and temperature in the 500-700
mbar range.

* SIV_2 (10.7 micron) - sensing temperature and ammonia in the 400-600 mbar
range.

* NEII_1 - (12.3 micron) - sensing temperature, ammonia, and stratospheric
ethane emission.

* NEII_2 - (13.0 micron) - primarily sensing tropospheric temperature in the
300-500 mbar region.

* Q1, Q2 and Q3 (17.6, 18.7 and 19.5 micron) - sensing tropospheric temperature
in the 100-300 mbar range.
