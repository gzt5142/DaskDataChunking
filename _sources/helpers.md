# Helper Scripts

This is a collection of helpers/demo scripts to show how we like to 
perform common tasks that might be replicated within any notebook 
in this repository:

```{tableofcontents}
```

## How to Use

Supposing that you want to start the dask cluster on the `nebari` cloud
hosting environment.  You could do that by hand using a dask `Gateway()`, 
or you could just:

```
%run StartNebariCluster.ipynb
```

That cell "magic" will run and load the named notebook within the context
of the notebook calling it.  It is similar to module loading in python, but
allows us to document helper operations in their own notebooks. 
