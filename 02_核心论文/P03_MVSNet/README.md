# MVSNet

MVSNet: Depth Inference for Unstructured Multi-view Stereo

## 论文与官方资源

- [MVSNet: Depth Inference for Unstructured Multi-view Stereo](https://arxiv.org/abs/1804.02505) · [直接打开 PDF](https://arxiv.org/pdf/1804.02505)
- [会议论文](https://openaccess.thecvf.com/content_ECCV_2018/html/Yao_Yao_MVSNet_Depth_Inference_ECCV_2018_paper.html)
- [官方代码](https://github.com/yoyo000/mvsnet)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | ECCV 2018 |
| 优先级 | A 多视图基础 |
| 训练方式 | 跨场景训练的多视图深度网络 |
| 模板依赖 | 不依赖人体模板 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** 有重叠的多张图像、相机内外参和深度范围；训练通常需要深度监督。

**输出：** 参考视图深度和置信信息，可进一步融合为表面。

## 重点学习

1. 可微单应性变换和深度假设。
2. Cost volume 的构造与多视图聚合。
3. 3D CNN 正则化、深度回归和融合。

## 对 BodyTrace 的建议用途

为当前轮廓与单目预测增加跨照片的视差证据。

## 适用条件与边界

皮肤弱纹理、45°间隔、遮挡和非刚性变姿会影响匹配；不能直接套用静态物体训练设置。

## 建议实践

在固定相机和静态人体数据上训练小基线，再分开增加角度、纹理和姿态困难。

## 复现状态

会议论文和作者代码已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
