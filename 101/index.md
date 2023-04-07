# Chunking 101

A gentle introduction to concepts and workflows. 

This introductory chapter will illustrate some key concepts for writing 
chunked data (in zarr format) to object storage in 'the cloud'.  We'll be
eventually be writing to an OSN storage device using the S3 API, although
you could, in theory, write anywhere (including a local file system). 

The illustration dataset will be PRISM(v2), accessed via its OpenDAP 
endpoint at <https://cida.usgs.gov/thredds/dodsC/prism_v2.html>


Buckle up... we will get up to speed fast. 

```{tableofcontents}
```


The dask performance report for the total conversion workflow is [here](../performance_reports/OpenDAP_to_S3-perfreport.html)

