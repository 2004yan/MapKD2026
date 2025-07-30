<div align="center">
<h1>MapKD: Unlocking Prior Knowledge with Multi-Level Cross-Modal Alignment and Distillation for Efficient Online HD Map Construction </h1>
  

</div >

![visualization](figs/teaser.jpg)

## Model

### Results on nuScenes-val set
We provide results on nuScenes-val set.

|    Range    |  Method   |  M  |   Div.   |   Ped.   |  Bound.  |   mIoU    |   Model    |   Config    |
|:-----------:|:--------:|:---:|:---:|:---:|:-----:|:--------:|:--------:|:--------:|
|  60 × 30 | HDMapNet | L+C | 45.9 | 30.5 | 56.8 | 44.40 | [ckpt](https://drive.google.com/file/d/1yYCRk_as7Vhvi_rL5BxqVrmEf_u7mB3b/view?usp=drive_link) | [cfg](config/nusc/baseline/baseline_60m.py) | 
|  60 × 30 | P-MapNet(SD+HD Prio.) | L+C | **54.2** | **41.3** | **63.7** | **53.07** | [ckpt](https://drive.google.com/file/d/1hr9QNRDOWmiqZcW2L5WY_o_0aIZFIo0W/view?usp=drive_link) | [cfg](config/nusc/hd_prior/hd_60m.py) | 
|  120 × 60 | HDMapNet | L+C | 53.6   |   37.8   |   57.1   |   49.50 | [ckpt](https://drive.google.com/file/d/1L_3whc53FmEdGh8Fn1EVS7xquX0_xHZJ/view?usp=drive_link) | [cfg](config/nusc/baseline/baseline_120m.py) | 
|  120 × 60 | P-MapNet(SD+HD Prio.) | L+C | **65.3** | **52.0** | **68.0** | **61.77** | [ckpt](https://drive.google.com/file/d/1MG10vfqFDnf4sYiDqdO2274LlQB670ne/view?usp=drive_link) | [cfg](config/nusc/hd_prior/hd_120m.py) | 
|  240 × 60 | HDMapNet | L+C | 40.0   |   26.8   |   42.6   |   36.47 | [ckpt](https://drive.google.com/file/d/1oKjYPXVxu0MwDzrOJ97r-0b2GBnKxK12/view?usp=drive_link) | [cfg](config/nusc/baseline/baseline_240m.py) | 
|  240 × 60 | P-MapNet(SD+HD Prio.) | L+C | **53.0** | **42.6** | **54.2** | **49.93** | [ckpt](https://drive.google.com/file/d/1lcA9U9oWKYM9X20gblBaG16I2DBLt2yU/view?usp=drive_link) | [cfg](config/nusc/hd_prior/hd_240m.py) | 


## Getting Started
- [Installation](docs/installation.md)
- [Train and Eval](docs/getting_started.md)
- [visualization](docs/visualization.md)


