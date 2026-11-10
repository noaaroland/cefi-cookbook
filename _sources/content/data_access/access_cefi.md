CEFI data
===
In November 2026, the NOAA/NEAP CEFI project transitioned to earthmover.io as the primary data access method for all users.
The data is currently still available through the PSL CEFI portal, supported by the PSL Thredds server and is available from cloud storage on directly AWS S3 and Google Cloud Storage via the NOAA NODD program.

However, the earthmover.io catalog and access services (ArrayLake and OPeNDAP) are much a faster and more streamlined way to access the data. All the variables in a region, experiment type, and time frequency are grouped together is a single catalog which you can open in single Python or R statement. From there you can access any subset of the data along any hyperslab needed for your analysis.

## The NOAA-CEFI earthmover.io catalog for data access

The entire public CEFI data catalog is available in the earthmover.io marketplace. If you are not associated with the CEFI project you can subscribe to the catalog and access the data through the earthmover.io ArrayLake and OPeNDAP services. If you are associated with the CEFI project you can access the data through this same mechanism, or you can setup authenticated access via your NOAA credentials, which will be required to access to certain pre-release and private data sets associated with the project.

We strongly encourage you to use the earthmover.io catalog, but we will maintain the information for other access routes for the time being.


---

##  Table of Content of Accessing CEFI Data
```{tableofcontents}
```
