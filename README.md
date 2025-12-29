# Advancing Off-Road Autonomous Driving: The Large-Scale ORAD-3D Dataset and Comprehensive Benchmarks

Repository for our paper ["Advancing Off-Road Autonomous Driving: The Large-Scale ORAD-3D Dataset and Comprehensive Benchmarks"](https://arxiv.org/abs/2510.16500).

## Introduction
A major bottleneck in off-road autonomous driving research lies in the scarcity of large-scale, high-quality datasets and benchmarks. To bridge this gap, we present ORAD-3D, which, to the best of our knowledge, is the largest dataset specifically curated for off-road autonomous driving. ORAD-3D covers a wide spectrum of terrains, including woodlands, farmlands, grasslands, riversides, gravel roads, cement roads, and rural areas, while capturing diverse environmental variations across weather conditions (sunny, rainy, foggy, and snowy) and illumination levels (bright daylight, daytime, twilight, and nighttime). Building upon this dataset, we establish a comprehensive suite of benchmark evaluations spanning five fundamental tasks: 2D free-space detection, 3D occupancy prediction, rough GPS-guided path planning, vision-language model-driven autonomous driving, and world model for off-road environments. Together, the dataset and benchmarks provide a unified and robust resource for advancing perception and planning in challenging off-road scenarios.

## Prepare data

The proposed off-road autonomous driving dataset ORAD-3D can be found [BaiduYun](XX) (code:XXXX, about 350GB). Extract and organize as follows:

```
|-- datasets
 |  |-- ORAD-3D
 |  |  |-- training
 |  |  |  |-- XX sequence   |-- calib
 |  |  |                    |-- sparse_depth
 |  |  |                    |-- dense_depth
 |  |  |                    |-- lidar_data
 |  |  |                    |-- local_path
 |  |  |                    |-- image_data
 |  |  |                    |-- occupancy
 |  |  |                    |-- gt_image
 |  |  |                    |-- gt_image_multi_seg
 |  |  |                    |-- scene_data (VLM)
 |  |  |                    |-- poses.txt
 ......
 |  |  |-- validation
 ......
 |  |  |-- testing
 ......
```

##  License

Our codes and dataset are released under the Apache 2.0 license.

# Bibtex
If this work is helpful for your research, please consider citing the following BibTeX entry.

```
@article{ORAD-3D,
  title={Advancing Off-Road Autonomous Driving: The Large-Scale ORAD-3D Dataset and Comprehensive Benchmarks},
  author={Chen Min, Jilin Mei, Heng Zhai, Shuai Wang, Tong Sun, Fanjie Kong, Haoyang Li, Fangyuan Mao, Fuyang Liu, Shuo Wang, Yiming Nie, Qi Zhu, Liang Xiao, Dawei Zhao, Yu Hu},
  journal={Arxiv},
  year={2025}
}
```

# Acknowledgement

Many thanks to these excellent open source projects:

- [ORFD](https://github.com/chaytonmin/Off-Road-Freespace-Detection) 

- [Off-Road Survey](https://github.com/chaytonmin/Survey-Autonomous-Driving-in-Unstructured-Off-Road-Environments) 

- [KISS-ICP](https://github.com/PRBonn/kiss-icp)

- [Qwen3-VL](https://github.com/QwenLM/Qwen3-VL)
