# EvGGS 复现评估结果

复现 [EvGGS](https://github.com/Mercerai/EvGGS) 论文的评估结果。

**环境**: PyTorch 1.12.1 + CUDA 11.6, RTX 3080 Ti (12GB)  
**模型**: `ft_evggs.pth` (OneDrive 提供的 finetuned checkpoint, 490K steps)  
**数据集**: Ev3D-S

## 快速结论

| 子任务 | 关键指标 | 复现 | 论文 | 对齐 |
|--------|----------|------|------|------|
| 深度估计 | AbsRel | 0.039 | 0.039 | ✅ |
| 强度重建 | SSIM | 0.967 | 0.969 | ✅ |
| 新视角合成 | PSNR | 20.22 | 27.95 | ❌ 差 ~8 dB |

## 文件

- `EVALUATION.md` — 完整评估报告
- `eval_val_ft_evggs.log` — val set 详细指标
- `eval_test_ft_evggs.log` — test set 详细指标
