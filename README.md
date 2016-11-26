[![](https://images.microbadger.com/badges/version/alexeyraga/ml-python-notebook.svg)](https://microbadger.com/images/alexeyraga/ml-python-notebook "Get your own version badge on microbadger.com")
[![](https://images.microbadger.com/badges/image/alexeyraga/ml-python-notebook.svg)](https://microbadger.com/images/alexeyraga/ml-python-notebook "Get your own image badge on microbadger.com")

# Jumpter Notebook for Machine Learning

A Jupiter Notebook containing `keras` and `theano` for experimenting with machine learning

## What it Gives You

* Fully-functional Jupyter Notebook
* Miniconda Python 3.x
* Preinstalled scientific packages: `keras`, `theano`, `hdf5`, `h5py`, `matplotlib`, etc.
* Unprivileged user `jovyan` (uid=1000, configurable, see options) in group `users` (gid=100) with ownership over `/home/jovyan` and `/opt/conda`

## Basic use

The following command starts a container with the Notebook server listening for HTTP connections on port 8888 with notebooks folder mounted to the current directory.

```
docker run -d -e -p 8888:8888 -v $PWD:/notebook alexeyraga/ml-python-notebook
```
