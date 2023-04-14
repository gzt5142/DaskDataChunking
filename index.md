# Data Chunking

"Chunking" large datasets is an essential workflow in the data peparation stage of
analysis.  Some of the large datasets are written with a chunking pattern which 
is optimized for writing (i.e. how they are created -- model outputs, etc), and
performs poorly for reading.  This depends on the analysis. 

Re-chunking is a useful strategy to re-write the dataset in such a way to optimize
a particular kind of analysis (i.e. time-series vs spatial). 



```{tableofcontents}
```

-----
Download the environment YAML file [here](env.yml)
