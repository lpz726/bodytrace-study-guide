# BodyTrace 算法与模型训练学习资料

围绕八视图自由人体曲面重建整理的中文学习索引，涵盖人体模型构造、法线和深度预测训练、多视图匹配，以及联合曲面优化。

原资料整理日期：2026 年 10 月 19 日。GitHub 链接版更新日期：2026 年 11 月 2 日。

## 直接阅读论文

点击下表的论文名称进入原文页面，点击“打开 PDF”直接阅读全文；“官方代码”和“阅读标注”也可直接跳转。每个论文文件夹均有带链接的 README，可在 GitHub 中直接阅读。

### 核心论文

| 论文 | 年份 | 原文 PDF | 官方代码 | 中文阅读标注 |
| --- | --- | --- | --- | --- |
| [DeepSDF](https://arxiv.org/abs/1901.05103) | 2019 | [打开 PDF](https://arxiv.org/pdf/1901.05103) | [官方代码](https://github.com/facebookresearch/DeepSDF) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P01_DeepSDF/README.md) |
| [PIFu](https://arxiv.org/abs/1905.05172) | 2019 | [打开 PDF](https://arxiv.org/pdf/1905.05172) | [官方代码与训练](https://github.com/shunsukesaito/PIFu) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P02_PIFu/README.md) |
| [MVSNet](https://arxiv.org/abs/1804.02505) | 2018 | [打开 PDF](https://arxiv.org/pdf/1804.02505) | [官方代码](https://github.com/yoyo000/mvsnet) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P03_MVSNet/README.md) |
| [DiffuStereo](https://arxiv.org/abs/2207.08000) | 2022 | [打开 PDF](https://arxiv.org/pdf/2207.08000) | [官方代码](https://github.com/DSaurus/DiffuStereo) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P04_DiffuStereo/README.md) |
| [DSINE](https://arxiv.org/abs/2403.00712) | 2024 | [打开 PDF](https://arxiv.org/pdf/2403.00712) | [官方代码与训练](https://github.com/baegwangbin/DSINE) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P05_DSINE/README.md) |
| [法线不确定性](https://arxiv.org/abs/2109.09881) | 2021 | [打开 PDF](https://arxiv.org/pdf/2109.09881) | [官方代码](https://github.com/baegwangbin/surface_normal_uncertainty) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P06_%E6%B3%95%E7%BA%BF%E4%B8%8D%E7%A1%AE%E5%AE%9A%E6%80%A7/README.md) |
| [MoGe](https://arxiv.org/abs/2410.19115) | 2025 | [打开 PDF](https://arxiv.org/pdf/2410.19115) | [官方代码](https://github.com/microsoft/MoGe) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P07_MoGe%20%E4%B8%8E%20MoGe-2/README.md) |
| [MoGe-2](https://arxiv.org/abs/2507.02546) | 2025 | [打开 PDF](https://arxiv.org/pdf/2507.02546) | [官方代码](https://github.com/microsoft/MoGe) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P07_MoGe%20%E4%B8%8E%20MoGe-2/README.md) |
| [Sapiens](https://arxiv.org/abs/2408.12569) | 2024 | [打开 PDF](https://arxiv.org/pdf/2408.12569) | [Sapiens 官方代码](https://github.com/facebookresearch/sapiens) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P08_Sapiens%20%E4%B8%8E%20Sapiens2/README.md) |
| [Sapiens2](https://arxiv.org/abs/2604.21681) | 2026 | [打开 PDF](https://arxiv.org/pdf/2604.21681) | [Sapiens2 官方代码](https://github.com/facebookresearch/sapiens2) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P08_Sapiens%20%E4%B8%8E%20Sapiens2/README.md) |
| [NeuS](https://arxiv.org/abs/2106.10689) | 2021 | [打开 PDF](https://arxiv.org/pdf/2106.10689) | [作者项目与代码入口](https://lingjie0206.github.io/papers/NeuS/index.htm) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P09_NeuS/README.md) |
| [MonoSDF](https://arxiv.org/abs/2206.00665) | 2022 | [打开 PDF](https://arxiv.org/pdf/2206.00665) | [官方代码](https://github.com/autonomousvision/monosdf) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P10_MonoSDF/README.md) |
| [SparseNeuS](https://arxiv.org/abs/2206.05737) | 2022 | [打开 PDF](https://arxiv.org/pdf/2206.05737) | — | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P11_SparseNeuS/README.md) |
| [ECON](https://openaccess.thecvf.com/content/CVPR2023/papers/Xiu_ECON_Explicit_Clothed_Humans_Optimized_via_Normal_Integration_CVPR_2023_paper.pdf) | 2023 | [打开 PDF](https://openaccess.thecvf.com/content/CVPR2023/papers/Xiu_ECON_Explicit_Clothed_Humans_Optimized_via_Normal_Integration_CVPR_2023_paper.pdf) | [官方代码](https://github.com/YuliangXiu/ECON) | [阅读标注](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87/P12_ECON/README.md) |

### 进阶论文

| 论文 | 年份 | 原文 PDF | 官方代码 | 中文阅读标注 |
| --- | --- | --- | --- | --- |
| [PIFuHD](https://arxiv.org/abs/2004.00452) | 2020 | [打开 PDF](https://arxiv.org/pdf/2004.00452) | [官方代码](https://github.com/facebookresearch/pifuhd) | [阅读标注](03_%E8%BF%9B%E9%98%B6%E8%AE%BA%E6%96%87/E01_PIFuHD/README.md) |
| [Neuralangelo](https://arxiv.org/abs/2306.03092) | 2023 | [打开 PDF](https://arxiv.org/pdf/2306.03092) | [官方项目与代码入口](https://research.nvidia.com/labs/dir/neuralangelo/) | [阅读标注](03_%E8%BF%9B%E9%98%B6%E8%AE%BA%E6%96%87/E02_Neuralangelo/README.md) |
| [MoGe-3](https://arxiv.org/abs/2607.17967) | 2026 | [打开 PDF](https://arxiv.org/pdf/2607.17967) | — | [阅读标注](03_%E8%BF%9B%E9%98%B6%E8%AE%BA%E6%96%87/E03_MoGe-3/README.md) |

## 基础课程与训练资料

### 基础课程

- [斯坦福 CS231n](https://cs231n.stanford.edu/schedule)
- [Szeliski Computer Vision 第二版](https://szeliski.org/Book/)
- [Multiple View Geometry 第二版](https://www.robots.ox.ac.uk/~vgg/hzbook/)
- [PyTorch3D 教程目录](https://pytorch3d.org/tutorials/)
- [PyTorch3D 网格变形实践](https://pytorch3d.org/tutorials/deform_source_mesh_to_target_mesh)
- [PyTorch3D 照片监督网格实践](https://pytorch3d.org/tutorials/fit_textured_mesh)

### 训练与数据构造

- [MoGe 官方训练教程](https://github.com/microsoft/MoGe/blob/main/docs/train.md)
- [Sapiens2 法线训练教程](https://github.com/facebookresearch/sapiens2/blob/main/docs/train/NORMAL.md)
- [Sapiens2 Pointmap 训练教程](https://github.com/facebookresearch/sapiens2/blob/main/docs/train/POINTMAP.md)
- [Omnidata 数据构造流程](https://github.com/EPFL-VILAB/omnidata)
- [THuman 数据说明](https://github.com/ytrock/THuman2.0-Dataset)

## 资料目录

| 目录 | 内容 |
| --- | --- |
| [01_基础材料](01_%E5%9F%BA%E7%A1%80%E6%9D%90%E6%96%99) | 计算机视觉、多视图几何与 PyTorch3D 教程 |
| [02_核心论文](02_%E6%A0%B8%E5%BF%83%E8%AE%BA%E6%96%87) | 12 个核心学习条目，包括 14 篇独立论文 |
| [03_进阶论文](03_%E8%BF%9B%E9%98%B6%E8%AE%BA%E6%96%87) | PIFuHD、Neuralangelo、MoGe-3 |
| [04_训练与数据资料](04_%E8%AE%AD%E7%BB%83%E4%B8%8E%E6%95%B0%E6%8D%AE%E8%B5%84%E6%96%99) | 官方训练教程与监督数据构造材料 |
| [05_学习计划](05_%E5%AD%A6%E4%B9%A0%E8%AE%A1%E5%88%92) | 分阶段实践路线及可填写的论文阅读模板 |
| [06_文献索引](06_%E6%96%87%E7%8C%AE%E7%B4%A2%E5%BC%95) | 全部可点击资源、JSON 索引与当前文件 SHA-256 |

## 下载交互阅读索引

点击 GitHub 页面上方 **Code → Download ZIP**，解压后双击 `index.html` 或 `00_开始阅读.html`，即可使用离线搜索、优先级筛选和逐篇标注。论文与官方代码链接需要联网。

## 建议学习顺序

DeepSDF / PIFu → DSINE / Sapiens2 → MVSNet / DiffuStereo → NeuS / MonoSDF → SparseNeuS。

跨数据模型训练、单对象优化和几何后处理在资料中分别标注。链接核验、训练流程可用和已经复现是不同状态；本资料包不声称完成这些方法的训练复现。

## 来源与使用

论文、模型和数据均指向作者或官方资源。中文导读和学习建议不替代原文；方法和训练信息按原整理日期保留。MVSNet 和 MonoSDF 的直接论文入口由作者官方仓库或项目页补充。

本仓库不包含完整论文 PDF、模型权重、训练数据或真人照片。第三方论文、代码、权重和数据的权利及许可归原作者或权利人所有，使用时分别查看原资源许可；THuman 的资料中保留了非商业研究用途限制说明。

`source-files.sha256.json` 记录来自原学习资料文件夹的文件身份；`06_文献索引/文件SHA256.txt` 为当前仓库内容的文件校验清单。
