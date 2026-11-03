# Navigating the Earthmover Catalog
When follow one of the links you will land in the catalog for the region, experiment type, and grid that contains your selected variable,  but you many not immediately see it because the catalog groups all the variables onto one page. That's actually good news, because when you follow the instructions for accessing the data you will have access to all the variables on that catalog page with only a few lines of code.  Use the menu in the upper right to choose how you want to access the data. For now, if you are an R user, pick the OPeNDAP option.

![Data access Menu](../../../images/access_data.png)

## Python

Choosing the Python will show you code snippets that will allow you to access the data using either zarr or xarray. For most people, [xarray](https://docs.xarray.dev/en/stable/user-guide/index.html) is the best option. It has many [high level features for Earth science data analysis](https://docs.xarray.dev/en/stable/user-guide/computation.html).

![Python code snippets](../../../images/python_snippet.png)


## OPeNDAP

Right now the best option for R access is OPeNDAP. Earthmover and the community are developing solutions for R access using the ArrayLake interface as is the standard for Python. Until those solutions are available, OPeNDAP is the best option. On the OPeNDAP data access page pay particular attention to the section showing how to read the data set in R.

![OPeNDAP code snippets](../../../images/opendap_snippets.png)

N.B. the OPeNDAP service is set to scale to 0 when not in use. In other words, if no requests are made for a period of time, the service will shut down. The service will automatically restart when a request is made, but there may be a small delay while it starts up. Once it has restarted all subsequent requests will begin returning data almost immediately.

