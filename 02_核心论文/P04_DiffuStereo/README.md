# DiffuStereo

DiffuStereo: High Quality Human Reconstruction via Diffusion-based Stereo Using Sparse Cameras

## 论文与官方资源

- [DiffuStereo: High Quality Human Reconstruction via Diffusion-based Stereo Using Sparse Cameras](https://arxiv.org/abs/2207.08000) · [直接打开 PDF](https://arxiv.org/pdf/2207.08000)
- [官方代码](https://github.com/DSaurus/DiffuStereo)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | ECCV 2022 |
| 优先级 | A 八视图重点精读 |
| 训练方式 | 稀疏人体多视图立体匹配网络训练与推理 |
| 模板依赖 | 学习重点为跨视图匹配；依赖相机及初始几何条件 |
| 项目关系 | 建议优先实验 |

## 输入与输出

**输入：** 稀疏人体多视图照片及相机参数；论文采用八相机设置。

**输出：** 多视图深度及融合的人体表面。

## 重点学习

1. 扩散式迭代立体匹配和深度修正。
2. 大基线与多分辨率网络。
3. 初始几何、立体约束和多视图融合。

## 对 BodyTrace 的建议用途

最贴近八个环绕视角的人体重建问题，重点比较其几何证据和当前 visual hull。

## 适用条件与边界

同步八相机数据不能直接等价于单人顺序转身照片；身体状态与标定仍是条件。

## 建议实践

先复核论文输入条件和官方示例，再拆出双视图深度模块做相同输入的对照。

## 复现状态

官方仓库训练章节仍有 TODO，45°权重说明仍有待提供项；不承诺完整训练复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
