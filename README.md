
## zarr store 

useful reading/links
* https://zarr-specs.readthedocs.io/en/latest/v3/core/v3.0.html#id21
* https://github.com/zarr-developers/zarr-python/issues/556
* https://medium.com/pangeo/cloud-performant-netcdf4-hdf5-with-zarr-fsspec-and-intake-3d3a3e7cb935
* https://github.com/zarr-developers/geozarr-spec
* https://github.com/ome/ome-zarr-py
* https://xarray-datatree.readthedocs.io/en/latest/
* napari generative zarr: [link to relevant part of PR](https://github.com/napari/napari/pull/6043/files#diff-ea6f2d7eb91873fb3e8eddee64be8697d0fb48c158d9a1f41b2e704627b36a63) and the [yt in napari generative zarr experiment](https://github.com/chrishavlin/napari_progressive_yt_experiment)
* https://github.com/manzt/napari-dzi-zarr zarr container for DZI for reading in napari
* https://janeliascicomp.github.io/pydantic-ome-ngff/ pydantic models of ome-ngff

## notes

### yt+zarr frontend-related 

* sph frontends: should be fairly straightforward to implement a frontend for an sph code with a zarr-hdf backend. 
* grid-based: uniform or stretched grids with no refinement also should be simple-ish 
* grid-based, refined: refined grids are a little trickier... could implement a custom zarr store that fills at a given refinement level (similar to a YTArbitraryGrid). this would kinda look like napari's generative zarr

### other zarr-related packages

* https://github.com/hms-dbmi/vizarr
