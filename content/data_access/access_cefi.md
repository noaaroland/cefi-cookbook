CEFI data
===
In November 2026, the NOAA/NEAP CEFI project transitioned to earthmover.io as the primary data access method for all users.
The data is currently still available through the PSL CEFI portal, supported by the PSL Thredds server and is available from cloud storage on directly AWS S3 and Google Cloud Storage via the NOAA NODD program.

However, the earthmover.io catalog and access services (ArrayLake and OPeNDAP) are much a faster and more streamlined way to access the data. All the variables in a region, experiment type, and time frequency are grouped together is a single catalog which you can open in single Python or R statement. From there you can access any subset of the data along any hyperslab needed for your analysis.

## The NOAA-CEFI earthmover.io catalog for data access

The entire public CEFI data catalog is available in the earthmover.io marketplace. If you are not associated with the CEFI project you can subscribe to the catalog and access the data through the earthmover.io ArrayLake and OPeNDAP services. If you are associated with the CEFI project you can access the data through this same mechanism, or you can setup authenticated access via your NOAA credentials, which will be required to access to certain pre-release and private data sets associated with the project.

We strongly encourage you to use the earthmover.io catalog, but we will maintain the information for other access routes for the time being.

### CEFI portal data access
The CEFI portal currently provides three ways to [access data](https://psl.noaa.gov/cefi_portal/#data_access), including:
- Direct [Thredds server catalog access](https://psl.noaa.gov/thredds/catalog/Projects/CEFI/regional_mom6/catalog.html)
- A list of variables in diffenrent formats (including HTML, JSON, and XML) 
- A data query generator that creates URLs, code snippets, download links, and data citation information
These three methods aim to meet a wide range of data needs for the public and researchers. Users are encouraged to explore the different options and choose the method that is most familiar and easy for them to use. 

### CEFI NODD data access
The cloud access methods (from the browser, from Python, and from R) will work from any computing resource, but they are particularly effective if you are using a computing resource associated with the same cloud vendor where the data are stored.
#### AWS S3
You can view the data on AWS S3 via the [AWS S3 Explorer](https://noaa-oar-cefi-regional-mom6-nwa-pds.s3.amazonaws.com/index.html) interface. In the following sections we will show you how to access the data directly from you Python and R scripts by reading the Kerchunk ZARR index files that accompany the cloud data.

#### Google Cloud Storage
You can view the data on Google Cloud Storage via the [cloud console]( https://console.cloud.google.com/storage/browser/noaa-oar-cefi-regional-mom6-nwa) interface. You must be signed into a Google account. Any account should have access. However, in the following sections we will show you how to access the data directly from you Python and R scripts by reading the Kerchunk ZARR index files that accompany the cloud data.


---

##  Table of Content of Accessing OPeNDAP Server
```{tableofcontents}
```
