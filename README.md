<div align="center">
<h1>MapKD: Unlocking Prior Knowledge with Multi-Level Cross-Modal Alignment and Distillation for Efficient Online HD Map Construction </h1>
  

</div >


## Model

### Results on nuScenes-val set
We provide results on nuScenes-val set.
|     Method      |     M      |   Div.   |   Ped.   |  Bound.  |   mIoU    |   mAP    |
|:---------------:|:----------:|:--------:|:--------:|:--------:|:---------:|:--------:|
|   HDMapNet      |     C      |  13.80   |  39.50   |  40.20   |   31.16   |   23.13  |
| PMapNet (C & SD) |   C+SD     |  23.70   |  44.04   |  43.30   |   37.01   |   27.84  |
| PMapNet (C & SD & HD) | C+SD+HD  |  24.61   |  45.03   |  43.34   |   37.66   |   33.63  |
| PMapNet (C & L & SD)   | C+L+SD   |  40.65   |  55.29   |  63.75   |   53.23   |   36.32  |
| **PMapNet (C & L & SD & HD)** | **C+L+SD+HD** | **41.70** | **56.60** | **64.80** | **54.36** | **45.46** |
| PMapNet* (C & sim-L & SD)  | C+sim-L+SD | 25.08  |  44.26   |  44.73   |   38.02   |   34.16  |
| PMapNet* (C & sim-L & SD & HD) | C+sim-L+SD+HD | 26.20 | 44.80 | 45.30 | 38.76 | 35.07 |
| Bevdistill (10 epochs)    |     C      |  15.00   |  40.90   |  41.10   | 32.33 (+1.17) | 24.99 (+1.86) |
| Unidistill (10 epochs)    |     C      |  14.39   |  40.20   |  41.40   | 32.00 (+0.84) | 25.44 (+2.31) |
| MapDistill (10 epochs)    |     C      |  16.20   |  40.50   |  41.60   | 32.77 (+1.61) | 26.90 (+3.77) |
| Bevdistill (30 epochs)    |     C      |  17.93   |  42.80   |  43.50   | 34.74 (+3.58) | 29.40 (+6.27) |
| Unidistill (30 epochs)    |     C      |  19.75   |  43.10   |  43.30   | 35.38 (+4.22) | 29.48 (+6.35) |
| MapDistill (30 epochs)    |     C      |  20.11   |  41.90   |  43.70   | 35.23 (+4.07) | 29.89 (+6.76) |
| **MapKD (Ours, 10 epochs)** |     C      | **25.40** | **44.40** | **43.71** | **37.84 (+6.68)** | **34.07 (+10.94)** |



## Getting Started
- [Installation](docs/installation.md)
- [Train and Eval](docs/getting_started.md)
- [visualization](docs/visualization.md)


