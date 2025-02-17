<img src="./assets/logo2.png" width = "320" height = "110" alt="logo" />

<div align="center"><img src="./assets/nm.gif" width = "100" height = "100" alt="nm" /><img src="./assets/bg.gif" width = "100" height = "100" alt="bg" /><img src="./assets/cl.gif" width = "100" height = "100" alt="cl" /></div>

------------------------------------------
🎉🎉🎉 **[*OpenGait*](https://openaccess.thecvf.com/content/CVPR2023/papers/Fan_OpenGait_Revisiting_Gait_Recognition_Towards_Better_Practicality_CVPR_2023_paper.pdf) has been accpected by CVPR2023 as a highlight paper！** 🎉🎉🎉

OpenGait is a flexible and extensible gait recognition project provided by the [Shiqi Yu Group](https://faculty.sustech.edu.cn/yusq/) and supported in part by [WATRIX.AI](http://www.watrix.ai).

## What's New
- **[May 2023]** A real gait recognition system [All-in-One-Gait](https://github.com/jdyjjj/All-in-One-Gait) provided by [Dongyang Jin](https://github.com/jdyjjj) is avaliable.
- [Apr 2023] [CASIA-E](datasets/CASIA-E/README.md) is supported by OpenGait.
- [Feb 2023] [HID 2023 competition](https://hid2023.iapr-tc4.org/) is open, welcome to participate. Additionally, tutorial for the competition has been updated in [datasets/HID/](./datasets/HID).
- [Dec 2022] Dataset [Gait3D](https://github.com/Gait3D/Gait3D-Benchmark) is supported in [datasets/Gait3D](./datasets/Gait3D).
- [Mar 2022] Dataset [GREW](https://www.grew-benchmark.org) is supported in [datasets/GREW](./datasets/GREW).

## Our Publications
- [**CVPR 2023**] LidarGait: Benchmarking 3D Gait Recognition with Point Clouds, [*Paper*](https://openaccess.thecvf.com/content/CVPR2023/papers/Shen_LidarGait_Benchmarking_3D_Gait_Recognition_With_Point_Clouds_CVPR_2023_paper.pdf), [*Dataset and Code(Coming Soon)*](https://lidargait.github.io).
- [**CVPR 2023 Highlight**] OpenGait: Revisiting Gait Recognition Toward Better Practicality, [*Paper*](https://openaccess.thecvf.com/content/CVPR2023/papers/Fan_OpenGait_Revisiting_Gait_Recognition_Towards_Better_Practicality_CVPR_2023_paper.pdf), [*Code*](configs/gaitbase).
- [**ECCV 2022**] GaitEdge: Beyond Plain End-to-end Gait Recognition for Better Practicality, [*Paper*](), [*Code*](configs/gaitedge/README.md).

## A Real Gait Recognition System: All-in-One-Gait
<div align="center">
       <img src="./assets/probe1-After.gif"  width = "455" height = "256" alt="probe1-After" />
</div>

The workflow of [All-in-One-Gait](https://github.com/jdyjjj/All-in-One-Gait) involves the processes of pedestrian tracking, segmentation and recognition.
See [here](https://github.com/jdyjjj/All-in-One-Gait) for details.

## Highlighted features
- **Mutiple Dataset supported**: [CASIA-B](http://www.cbsr.ia.ac.cn/english/Gait%20Databases.asp), [OUMVLP](http://www.am.sanken.osaka-u.ac.jp/BiometricDB/GaitMVLP.html), [HID](http://hid2022.iapr-tc4.org/), [GREW](https://www.grew-benchmark.org), [Gait3D](https://github.com/Gait3D/Gait3D-Benchmark), and [CASIA-E](https://www.scidb.cn/en/detail?dataSetId=57be0e918db743279baf44a38d013a06).
- **Multiple Models Support**: We reproduced several SOTA methods, and reached the same or even the better performance. 
- **DDP Support**: The officially recommended [`Distributed Data Parallel (DDP)`](https://pytorch.org/tutorials/intermediate/ddp_tutorial.html) mode is used during both the training and testing phases.
- **AMP Support**: The [`Auto Mixed Precision (AMP)`](https://pytorch.org/tutorials/recipes/recipes/amp_recipe.html?highlight=amp) option is available.
- **Nice log**: We use [`tensorboard`](https://pytorch.org/docs/stable/tensorboard.html) and `logging` to log everything, which looks pretty.

## Getting Started


Please see [0.get_started.md](docs/0.get_started.md). We also provide the following tutorials for your reference:
- [Prepare dataset](docs/2.prepare_dataset.md)
- [Detailed configuration](docs/3.detailed_config.md)
- [Customize model](docs/4.how_to_create_your_model.md)
- [Advanced usages](docs/5.advanced_usages.md) 

## Model Zoo
Results and models are available in the [model zoo](docs/1.model_zoo.md).


## Authors:
**Open Gait Team (OGT)**
- [Chao Fan (樊超)](https://chaofan996.github.io), 12131100@mail.sustech.edu.cn
- [Chuanfu Shen (沈川福)](https://faculty.sustech.edu.cn/?p=95396&tagid=yusq&cat=2&iscss=1&snapid=1&orderby=date), 11950016@mail.sustech.edu.cn
- [Junhao Liang (梁峻豪)](https://faculty.sustech.edu.cn/?p=95401&tagid=yusq&cat=2&iscss=1&snapid=1&orderby=date), 12132342@mail.sustech.edu.cn

## Acknowledgement
- GLN: [Saihui Hou (侯赛辉)](http://home.ustc.edu.cn/~saihui/index_english.html)
- GaitGL: [Beibei Lin (林贝贝)](https://scholar.google.com/citations?user=KyvHam4AAAAJ&hl=en&oi=ao)
- GREW: [GREW TEAM](https://www.grew-benchmark.org)

## Citation
```
@InProceedings{Fan_2023_CVPR,
    author    = {Fan, Chao and Liang, Junhao and Shen, Chuanfu and Hou, Saihui and Huang, Yongzhen and Yu, Shiqi},
    title     = {OpenGait: Revisiting Gait Recognition Towards Better Practicality},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2023},
    pages     = {9707-9716}
}
```

**Note:**
This code is only used for **academic purposes**, people cannot use this code for anything that might be considered commercial use.
