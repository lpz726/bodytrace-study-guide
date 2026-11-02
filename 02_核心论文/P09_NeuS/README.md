# NeuS

NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-view Reconstruction

## 论文与官方资源

- [NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-view Reconstruction](https://arxiv.org/abs/2106.10689) · [直接打开 PDF](https://arxiv.org/pdf/2106.10689)
- [作者项目与代码入口](https://lingjie0206.github.io/papers/NeuS/index.htm)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | NeurIPS 2021 |
| 优先级 | A 连续曲面优化基础 |
| 训练方式 | 主要针对单个静态对象或场景优化神经场 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** 多视图照片和相机参数。

**输出：** SDF 场、颜色场及提取的表面网格。

## 重点学习

1. SDF 到体渲染权重的转换与几何偏差。
2. 射线采样、颜色网络和 Eikonal 正则。
3. 用图像损失优化连续曲面并提取网格。

## 对 BodyTrace 的建议用途

为照片约束自由表面建立可微优化框架。

## 适用条件与边界

单对象优化不同于训练一个能泛化到所有人的前馈模型；人体需处理跨照片形变。

## 建议实践

用已知相机、静态几何和独立 GT 运行一个对象，分别比较颜色与几何指标。

## 复现状态

论文与作者项目已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
