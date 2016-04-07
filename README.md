# WRF Plot
# wrfplot.py

Python script to plot various WRF-ARW output. Written for Python 2.x

# Currently plots

- 2m temp and wind barbs
- MSLP only
- Total accumulated precipitation
- Total precipitation
- Convective precipitation
- 2m dew point temperature
- Relative humidity
- Snow accumulation
- Hail accumulation
- Simulated reflectivity
- Composite reflectivity
- LCL
- Theta-e
- Upper level charts (geopotential height, wind barbs and temperature)
- H7-H5 lapse rates
- 500mb absolute vorticity

Also supports saving plots as PNG images.

Example Usage: wrfplot.py --infile filename.nc --sfc --tunit C --td --ppn --punit mm

Use wrfplot.py --help to see all possible options.

# Future improvements

- Plotting of severe weather parameters such as; CAPE, SRH, 0-6 SHR etc
- Plotting of soundings at a given latitude and longitude
- Get data for given latitude and longitude such as max/min of variables
- Revise reflectivity routine. Possibly use FORTRAN routines to compute reflectivity
- Tidy code up to improve efficiency

# Known Issues

- Simulated and Composite Reflectivity calculations not working correctly. Method used is for Ferrier, WSM5, fixed intercept      microphysics
- Contour/Color bar levels for various parameters need revising

Feel free to use and modify this script but please give credit when used. 
