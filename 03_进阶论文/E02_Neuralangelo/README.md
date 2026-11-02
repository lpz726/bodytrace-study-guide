# Neuralangelo

Neuralangelo: High-Fidelity Neural Surface Reconstruction

## 论文与官方资源

- [Neuralangelo: High-Fidelity Neural Surface Reconstruction](https://arxiv.org/abs/2306.03092) · [直接打开 PDF](https://arxiv.org/pdf/2306.03092)
- [官方项目与代码入口](https://research.nvidia.com/labs/dir/neuralangelo/)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | CVPR 2023 |
| 优先级 | C 高细节优化选读 |
| 训练方式 | 单场景神经表面优化 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 后续拓展 |

## 输入与输出

**输入：** 静态场景多视图图像和相机。

**输出：** 高细节隐式表面及网格。

## 重点学习

1. 多分辨率 hash grid。
2. 数值梯度和曲率正则。
3. 粗到细训练课程。

## 对 BodyTrace 的建议用途

研究细节、平滑和优化稳定性。

## 适用条件与边界

静态场景/视频采集条件不等于八张非刚性人体照片。

## 建议实践

固定采集与预算，比较编码和正则对独立几何误差的影响。

## 复现状态

官方项目和论文已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
