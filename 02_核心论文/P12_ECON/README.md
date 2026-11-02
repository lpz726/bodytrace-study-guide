# ECON

ECON: Explicit Clothed Humans Optimized via Normal Integration

## 论文与官方资源

- [ECON: Explicit Clothed Humans Optimized via Normal Integration](https://openaccess.thecvf.com/content/CVPR2023/papers/Xiu_ECON_Explicit_Clothed_Humans_Optimized_via_Normal_Integration_CVPR_2023_paper.pdf) · [直接打开 PDF](https://openaccess.thecvf.com/content/CVPR2023/papers/Xiu_ECON_Explicit_Clothed_Humans_Optimized_via_Normal_Integration_CVPR_2023_paper.pdf)
- [官方代码](https://github.com/YuliangXiu/ECON)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | CVPR 2023 |
| 优先级 | B 法线积分组件精读 |
| 训练方式 | 学习型观测与法线积分、几何拼合相结合 |
| 模板依赖 | 原方法依赖 SMPL-X |
| 项目关系 | 建议研究组件；不是无模板直接替代 |

## 输入与输出

**输入：** 单张人体照片、预测法线及 SMPL-X 基础几何。

**输出：** 经法线积分与拼合得到的着衣人体表面。

## 重点学习

1. d-BiNI 与低频位置/高频法线约束。
2. 轮廓边界、积分漂移和前后表面拼合。
3. 显式、隐式几何组件的组合。

## 对 BodyTrace 的建议用途

借鉴当前外包络基础上的受约束法线积分。

## 适用条件与边界

迁移到无模板路线时，需要重新设计位置、遮挡和边界约束来源。

## 建议实践

以已知外包络替代低频参考做小实验，检查凹陷恢复和低频漂移。

## 复现状态

论文与官方代码已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
