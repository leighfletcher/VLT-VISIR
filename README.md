# VLT VISIR Observations

The VLT Imager and Spectrometer for the mid-infrared (VISIR Lagage et al., 2004) on the 8.2-m diameter Melipal telescope has been used to study Jupiter since 2006.  

VISIR returned to the 8.2 m UT3/Melipal telescope in 2015 after a 3 yr refurbishment, and was subsequently used to provide thermal-infrared support for observations from Juno and JWST. 

The new 1024×1024 Raytheon Aquarius IBC detector offers a pixel size of 0"0453/pixel over a 38″×38″ field of view. This is smaller than the disk of Jupiter at opposition, so observations are typically taken in 2 modes:  one where we chop to the south (leaving the northern hemisphere visible), and one where we chop to the north.  

In each observation block, we cycle through 9 filters in the 5-20 µm range, sounding Jupiter's temperatures and aerosols from the troposphere (2-3 bars at 5 µm) to the stratosphere (1-10 mbar at 7.9 µm).

Jupiter is detected differentially on top of the sky background, so we have to both nod (by 60") and chop (by 25") to remove thermal background from the data.  The chop-throw is smaller that Jupiter's 40-50" angular size, meaning that data will exhibit the negative "B beam" obscuring one hemisphere or the other.  

## Data Processing

Quick-look observations for each observing block are processed and stored here - the underlying data is available on request.  The following processing steps have been performed:
1. Reconstruct the image by combining chops and nods.
1. Use `Planetmapper` to fit the limb and assign geometry.
1. Window the detector, separating the two halves (master and slave).
1. Destripe the two halves of the detector and recombine.
1. Remove the corrupted overlap region between master and slave detectors.
1. Shift and add back in the negative beam, flagging regions of imperfect limb correction.

In the quick-look images, you'll see two white regions:  the removed central row; and the region omitted due to imperfect correction of the negative beam.  Data "interior" to the limb arc should be treated with caution, it is corrected for aesthetic purposes and should not be used for science.  

## Wavelengths

The filenames provide the time of the observation and the wavelength via the
following codes:  

* M-Band (5 micron) - sensing deep cloud opacity.

* J7.9 (7.9 micron) - sending stratospheric temperature near 10-20 mbar via methane emission.

* PAH1 (8.6 micron) - sensing aerosol opacity and temperature in the 500-700 mbar range.

* SIV_2 (10.7 micron) - sensing temperature and ammonia in the 400-600 mbar range.

* NEII_1 - (12.3 micron) - sensing temperature, ammonia, and stratospheric ethane emission.

* NEII_2 - (13.0 micron) - primarily sensing tropospheric temperature in the 300-500 mbar region.

* Q1, Q2 and Q3 (17.6, 18.7 and 19.5 micron) - sensing tropospheric temperature in the 100-300 mbar range.

## Data Record

| Date | Comment | Publication | Quicklook |
|---|---|---|---|
| 2025-01-27 | South near PJ69 | -  | ![Quicklook](quicklook/2025-01-27T00:41:49.0755_Jupiter.clean.png)  |
| 2025-01-27 | North near PJ69 | -  | ![Quicklook](quicklook/2025-01-27T02:37:32.5628_Jupiter.clean.png)  |
| 2025-01-25 | South near PJ69 | -  | ![Quicklook](quicklook/2025-01-25T01:25:10.4793_Jupiter.clean.png)  |
| 2025-01-24 | South SEB Outbreak | -  | ![Quicklook](quicklook/2025-01-24T01:42:49.1527_Jupiter.clean.png)

