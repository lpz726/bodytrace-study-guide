# MoGe 与 MoGe-2

MoGe / MoGe-2

## 论文与官方资源

- [MoGe: Unlocking Accurate Monocular Geometry Estimation for Open-Domain Images with Optimal Training Supervision](https://arxiv.org/abs/2410.19115) · [直接打开 PDF](https://arxiv.org/pdf/2410.19115)
- [MoGe-2: Accurate Monocular Geometry with Metric Scale and Sharp Details](https://arxiv.org/abs/2507.02546) · [直接打开 PDF](https://arxiv.org/pdf/2507.02546)
- [官方代码](https://github.com/microsoft/MoGe)
- [训练教程](https://github.com/microsoft/MoGe/blob/main/docs/train.md)
- [法线头说明](https://github.com/microsoft/MoGe/blob/main/docs/normal.md)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | MoGe：CVPR 2025；MoGe-2：2025 论文 |
| 优先级 | A 当前模型训练 |
| 训练方式 | 跨数据几何预测模型的监督训练与微调 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 当前项目使用 MoGe-2 观测；训练方案为学习建议 |

## 输入与输出

**输入：** RGB；训练数据可包括深度、归一化相机内参、法线及有效区域。

**输出：** 点图、深度、尺度相关输出及法线等，随具体版本和模型头变化。

## 重点学习

1. Affine-invariant pointmap 与尺度、平移歧义。
2. 全局和多尺度局部几何监督。
3. 米制尺度、标签质量和真实/合成混合训练。
4. 法线头标签来源和平方角度损失。

## 对 BodyTrace 的建议用途

理解并微调当前几何观测器，优先研究人体数据监督与损失而非仅替换权重。

## 适用条件与边界

当前项目对深度采用相对 affine 观测；预测米制能力不等于已在本项目获得独立标定精度。

## 建议实践

固定相同人体训练/测试划分，对照只训练预测头与联合微调骨干。

## 复现状态

官方仓库已公开 v1/v2 训练文档；本资料包未训练。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
