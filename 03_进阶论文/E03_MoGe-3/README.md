# MoGe-3

Fine-Detail Monocular Geometry Estimation with Self-Guided Sparse Volumetric Refinement

## 论文与官方资源

- [Fine-Detail Monocular Geometry Estimation with Self-Guided Sparse Volumetric Refinement](https://arxiv.org/abs/2607.17967) · [直接打开 PDF](https://arxiv.org/pdf/2607.17967)
- [官方训练文档](https://github.com/microsoft/MoGe/blob/main/docs/train.md)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | 2026 预印本 |
| 优先级 | C MoGe-2 之后选读 |
| 训练方式 | 预训练 MoGe-2 上的三维细化训练 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 后续拓展；当前项目未接入 |

## 输入与输出

**输入：** RGB 和初始点图特征；训练需几何监督。

**输出：** 细化后的单目几何。

## 重点学习

1. 点图向稀疏三维体积的提升。
2. 三维细化与二维特征混合的区别。
3. 多次迭代监督和细化数据管线。

## 对 BodyTrace 的建议用途

研究三维空间中的局部几何 refinement。

## 适用条件与边界

新模型在本项目人体上的收益需要独立实验。

## 建议实践

使用完全相同的人体测试集比较 v2/v3，分开评价整体与局部误差。

## 复现状态

2026 论文与官方训练文档已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
