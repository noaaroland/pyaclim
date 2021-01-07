# pyaclim
These are some notebooks I used to manipulate some ACLIM data to add centroid lat/lon values to an existing netCDF file.

1. **regions.ipynb** - assumes you know the lat/lon locations and just rewrites the data as a giant CSV file.
1. **regions2.ipynb** - also assumes you know the lat/lon locations, but uses pandas to manipulate the data to add the lat/lon. There are steps to reset and set the indies of the data frame mostly to make it easier to mainpulate the data, but also because the pocean package wants a "flat" data frame.
1. **regions3.ipynb** -  is the entire process. It shows how to find the centroids from the shape file, create data arrays from the result, add those data arrays to the data set read from the file and write the file back out. All using xarray rather than pandas.
