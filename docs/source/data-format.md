# Interoperable data formats

The diversity of raw data file formats generated by different sonar systems is a major obstacle toward integrative analysis of ocean sonar data at large scales. Echopype addresses this problem by providing tools for converting and standardizing data from manufacturer-specific formats into the **[netCDF](https://www.unidata.ucar.edu/software/netcdf/) data model**, so that data from different instruments are interoperable. NetCDF is the [current defacto standard](https://clouds.eos.ubc.ca/~phil/courses/parallel_python/02_xarray_zarr.html) in climate research and is supported by many powerful Python packages for efficient computation, of which echopype takes advantage extensively.

The section [**Raw converted data**](data-format:raw-data) details how echopype handles and represents data unpacked and standardized ("converted") from the raw files generated by the sonar instruments. Echopype follows the [ICES SONAR-netCDF4 convention version 1](http://www.ices.dk/sites/pub/Publication%20Reports/Cooperative%20Research%20Report%20(CRR)/CRR341.pdf) to create interoperable data, with exceptions as described in [echopype-specific modifications](data-format:mod-to-sonart-netcdf4).

The section [**Processed data**](data-format:processed-data) provides information for the format of derived data products, such as calibrated `Sv` data. These data products are based on the general netCDF data model.
