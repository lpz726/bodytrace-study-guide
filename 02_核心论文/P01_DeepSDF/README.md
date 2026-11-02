# DeepSDF

DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation

## 论文与官方资源

- [DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation](https://arxiv.org/abs/1901.05103) · [直接打开 PDF](https://arxiv.org/pdf/1901.05103)
- [官方代码](https://github.com/facebookresearch/DeepSDF)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | CVPR 2019 |
| 优先级 | A 基础必读 |
| 训练方式 | 跨形状监督训练；新对象可优化潜变量 |
| 模板依赖 | 不以 SMPL 人体模板为核心输入 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** 训练：三维查询点、SDF 标签、形状身份；拟合新对象：部分几何观测。

**输出：** 连续 SDF、零水平集网格、形状潜变量。

## 重点学习

1. SDF 的符号、距离和零水平集。
2. 表面附近与空间内的采样及截断距离损失。
3. Auto-decoder 和形状潜变量的联合训练。
4. 新对象潜变量优化与网格提取。

## 对 BodyTrace 的建议用途

为自由曲面选择连续表示，研究用人体扫描训练低频形状先验。

## 适用条件与边界

本身不是从照片直接重建人体的完整方案；隐藏区域补全受训练分布影响。

## 建议实践

先拟合一个有独立网格真值的对象，比较采样密度和损失截断对表面误差的影响。

## 复现状态

官方代码入口已核验；本资料包未执行训练或复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
