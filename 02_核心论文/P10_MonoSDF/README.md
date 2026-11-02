# MonoSDF

MonoSDF: Exploring Monocular Geometric Cues for Neural Implicit Surface Reconstruction

## 论文与官方资源

- [MonoSDF: Exploring Monocular Geometric Cues for Neural Implicit Surface Reconstruction](https://arxiv.org/abs/2206.00665) · [直接打开 PDF](https://arxiv.org/pdf/2206.00665)
- [论文与作者项目](https://niujinshuchong.github.io/monosdf/)
- [官方代码](https://github.com/autonomousvision/monosdf)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | NeurIPS 2022 |
| 优先级 | A 当前联合优化重点 |
| 训练方式 | 针对单个静态场景的几何先验辅助联合优化 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** 多视图 RGB、相机、单目深度与法线线索。

**输出：** 联合优化的连续表面及网格。

## 重点学习

1. 深度、法线、RGB 对 SDF 的联合监督。
2. 深度尺度与偏移对齐。
3. 几何损失、Eikonal 与不同隐式表示的比较。

## 对 BodyTrace 的建议用途

最直接参考：将 MoGe/Sapiens 观测纳入联合几何优化。

## 适用条件与边界

单目预测先验不能充当独立真值；静态场景结果不直接代表转身人体。

## 建议实践

在相同输入上做 RGB、RGB+深度、RGB+法线和全部线索四组消融。

## 复现状态

作者项目和官方代码已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
