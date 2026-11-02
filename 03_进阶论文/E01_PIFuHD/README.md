# PIFuHD

PIFuHD: Multi-Level Pixel-Aligned Implicit Function for High-Resolution 3D Human Digitization

## 论文与官方资源

- [PIFuHD: Multi-Level Pixel-Aligned Implicit Function for High-Resolution 3D Human Digitization](https://arxiv.org/abs/2004.00452) · [直接打开 PDF](https://arxiv.org/pdf/2004.00452)
- [作者项目](https://shunsukesaito.github.io/PIFuHD/)
- [官方代码](https://github.com/facebookresearch/pifuhd)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | CVPR 2020 |
| 优先级 | C 多尺度选读 |
| 训练方式 | 多层级人体隐式预测网络 |
| 模板依赖 | 核心为图像条件隐式函数 |
| 项目关系 | 后续拓展 |

## 输入与输出

**输入：** 单张人体照片及法线等辅助线索。

**输出：** 多尺度隐式人体表面。

## 重点学习

1. Coarse-to-fine 层级。
2. 全局形状与局部高分辨率特征。
3. 法线辅助预测。

## 对 BodyTrace 的建议用途

学习整体比例和细节分支的网络构造。

## 适用条件与边界

高图像分辨率与密集网格不等于毫米准确度；不能默认官方训练流程完整。

## 建议实践

对照单尺度和多尺度特征，报告局部几何误差。

## 复现状态

论文、官方项目与代码已核验；完整训练流程未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
