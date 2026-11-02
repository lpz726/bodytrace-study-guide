# 法线不确定性

Estimating and Exploiting the Aleatoric Uncertainty in Surface Normal Estimation

## 论文与官方资源

- [Estimating and Exploiting the Aleatoric Uncertainty in Surface Normal Estimation](https://arxiv.org/abs/2109.09881) · [直接打开 PDF](https://arxiv.org/pdf/2109.09881)
- [官方代码](https://github.com/baegwangbin/surface_normal_uncertainty)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | ICCV 2021 |
| 优先级 | A 可靠性与加权 |
| 训练方式 | 联合预测法线与偶然不确定性的监督训练 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** RGB、法线标签、有效区域。

**输出：** 法线方向及其概率分布参数。

## 重点学习

1. 单位球面上的方向概率分布。
2. 负对数似然与方向、不确定性联合训练。
3. 困难像素、边界与可靠性评估。

## 对 BodyTrace 的建议用途

将规则式法线支持权重升级为可学习、可校准的可靠性估计。

## 适用条件与边界

预测不确定性不是自动校准的正确率；需要在人体和目标拍摄条件上验证。

## 建议实践

比较无加权、人工权重和学习权重对独立法线误差及最终三维误差的影响。

## 复现状态

论文与官方代码已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
