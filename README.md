# Breyo Observatory Data Reduction & Analysis Pipeline

The repository collects code and documentation used to process imaging and
spectroscopy from the [Siena College](http://siena.edu) [Breyo
Observatory](https://www.siena.edu/departments/physics-and-astronomy/breyo-observatory)
0.7-meter optical telescope.

## Installing

```
conda create --name breyo python=3.6
conda activate breyo
conda install -c astropy astropy ccdproc photutils 
conda install jupyterlab ipython
```

Building astrometry.net requires a little work (should use a Docker container),
but I had to do

```
brew install cairo
brew install netpbm
export NETPBM_LIB="-L/usr/local/lib -lnetpbm"
export NETPBM_INC=-I/usr/local/include/netpbm
export CAIRO_LIB="-L/usr/local/lib -lcairo"
export CAIRO_INC=-I/usr/local/include/cairo
make
make extra
make install INSTALL_DIR=/usr/local/astrometry
```


## Authors

* [**Rose Finn**](https://github.com/rfinn)
* [**John Moustakas**](https://github.com/moustakas)

## Acknowledgments

