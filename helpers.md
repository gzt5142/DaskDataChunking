# Helper Scripts

This is a collection of helpers/demo scripts to show how we like to 
perform common tasks that might be replicated within any notebook 
in this repository.

```{tableofcontents}
```

## How to Use

Supposing that you want to start the dask cluster on the `nebari` cloud
hosting environment.  You could do that by hand using a dask `Gateway()`, 
or you could use our boilerplate:

```
%run StartNebariCluster.ipynb
```

That cell "magic" will run and load the named notebook within the context
of the notebook calling it.  It is similar to module loading in python, but
allows us to document helper operations in their own notebooks. 

This mechanism allows us to start the cluter in exactly the same way every
time, and with only one line of code in each notebook that needs a cluster. 
See the {doc}`StartNebariCluster` itself to see how you might modify its
behavior without having to rewrite or replicate it. 

## Why? 

This mechanism is similar to a more typical python module import. We like
the running of external notebooks because it allows us to use jupyter-book
friendly explanations of each helper and its use.  And it also prevents 
notebooks from having to modify `sys.path` in order to import modules using
the standard mechanism. 