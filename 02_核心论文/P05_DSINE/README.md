# DSINE

Rethinking Inductive Biases for Surface Normal Estimation

## 论文与官方资源

- [Rethinking Inductive Biases for Surface Normal Estimation](https://arxiv.org/abs/2403.00712) · [直接打开 PDF](https://arxiv.org/pdf/2403.00712)
- [官方代码与训练](https://github.com/baegwangbin/DSINE)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | CVPR 2024 |
| 优先级 | A 法线模型重点 |
| 训练方式 | 监督法线网络训练与微调 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 建议优先实验；当前 free-body 未调用 DSINE |

## 输入与输出

**输入：** RGB、相机内参；训练需要法线标签及有效掩码。

**输出：** 逐像素表面法线；部分模型另有不确定性。

## 重点学习

1. 将逐像素相机射线输入模型。
2. 通过相邻法线相对旋转进行迭代细化。
3. 相机内参、数据增强和损失构造。

## 对 BodyTrace 的建议用途

设计具备相机几何归纳偏置的人体法线基线。

## 适用条件与边界

模型输出法线还需融合成表面；官方简易训练示例规模不等于论文完整训练。

## 建议实践

从 baseline_normal 开始，使用相同人体数据比较是否引入射线及相对旋转。

## 复现状态

官方 README 有训练、自定义数据和深度生成法线说明；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
