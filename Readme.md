# Installation

```bash
# Create a clean environment
pixi init

# Install development version of yt
pixi add --git https://github.com/cphyc/yt.git --branch octree-particles yt --pypi 

# Download package to load cutouts
pixi add --git https://github.com/AnatoleStorck/yt_derived_fields.git --branch improve-loader yt_derived_fields --pypi
pixi add cython_fortran_file --pypi
```

# Use
```python
from yt_derived_fields.cutouts.loader import load_cutout

ds = load_cutout("path/to/halo_cutout.bin")
```