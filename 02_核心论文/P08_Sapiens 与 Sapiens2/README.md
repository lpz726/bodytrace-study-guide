# Sapiens 与 Sapiens2

Sapiens / Sapiens2

## 论文与官方资源

- [Sapiens: Foundation for Human Vision Models](https://arxiv.org/abs/2408.12569) · [直接打开 PDF](https://arxiv.org/pdf/2408.12569)
- [Sapiens2](https://arxiv.org/abs/2604.21681) · [直接打开 PDF](https://arxiv.org/pdf/2604.21681)
- [Sapiens 官方代码](https://github.com/facebookresearch/sapiens)
- [Sapiens2 官方代码](https://github.com/facebookresearch/sapiens2)
- [法线训练教程](https://github.com/facebookresearch/sapiens2/blob/main/docs/train/NORMAL.md)
- [Pointmap 训练教程](https://github.com/facebookresearch/sapiens2/blob/main/docs/train/POINTMAP.md)

## 阅读标注

| 项目 | 内容 |
| --- | --- |
| 年份与发表信息 | Sapiens：2024；Sapiens2：2026 |
| 优先级 | A 人体专用微调 |
| 训练方式 | 人体领域预训练骨干与稠密任务头微调 |
| 模板依赖 | 不以 SMPL 为必需预测输入 |
| 项目关系 | 当前项目使用一代 Sapiens；Sapiens2 为后续实验建议 |

## 输入与输出

**输入：** 人体 RGB；法线任务需单位向量标签；pointmap 任务需相机坐标系逐像素三维点。

**输出：** 按任务预测分割、法线、pointmap 等。

## 重点学习

1. 人体领域预训练与高分辨率特征。
2. 任务头、训练配置、数据集类与微调。
3. 法线和 pointmap 的标签坐标约定。

## 对 BodyTrace 的建议用途

构造人体专用几何观测网络，以较小预训练模型和自有数据开始微调。

## 适用条件与边界

人体法线模型不是肌肉解剖测量模型；Sapiens2 不代表当前项目已接入。

## 建议实践

先用官方 NORMAL 数据格式微调，再与未微调模型在按人隔离的测试集比较。

## 复现状态

Sapiens2 官方 NORMAL/POINTMAP 训练教程已核验；本资料包未复现。

[返回完整论文目录](../../README.md)

论文方法及原始资料按原学习索引保留；优先级和实践任务为项目学习建议。
