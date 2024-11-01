# DistortoCorrect Stitcher

DistortoCorrect Stitcher is a tool designed to accurately stitch image tiles with distortion correction for microscopy. This repository contains a Jupyter notebook, `distortCorrectStitcher.ipynb`, which provides a full workflow for stitching and distortion correction. The details of the algorithm and implementation can be found in our forthcoming publication.

## Features
- **Input Format**: Image tiles in float32 format with dimensions `[tile, color, y, x]`. Each tile should be `2048 x 2048` pixels. Additionally, the global positions should be provided in an `n x 2` array, where each row contains the `y` and `x` coordinates (top-left corner) of each tile.
- **Output Format**: An assembled TIFF file in the `tyx` format, compatible with Fiji (ImageJ) for further analysis.

## Requirements
This project requires Python 3.10 and the following packages:
- torch==2.4
- cupy==13.3
- cucim==24.10
- cuda==12.5
- networkx==3.4
- numba==0.60
- tifffile==2024.9.20
- scikit-learn==1.5.2
- scikit-image==0.24

## Usage
The `distortCorrectStitcher.ipynb` notebook provides a complete stitching process with distortion correction.

## License
This project is licensed under the Apache License, Version 2.0. Portions of code included in this project were originally licensed under the MIT License and authored by Johan Öfverstedt (2021). These portions have been modified and incorporated into this work. The full text of the MIT License is included in the root folder, in compliance with the original license terms.

## Citation
If you use this tool in your research, please cite our work as specified in the [future publication reference here].

## Documentation
Full details of the method and examples can be found in the paper [to be added].
