# 文件名 | 中文说明（紧凑表格）

文件/路径 | 中文说明
---|---
MacroAddingMicrostructure.m | 示例脚本：如何在计算得到的频移图上加入微结构效应（用于生成图9）
MacrocreateQSMpipelineAndCompareHighResLowRes.m | 示例脚本：使用模拟数据在高/低分辨率下创建 QSM 流程并比较
MacroCreateSimulationData.m | 示例脚本：如何使用代码和弛豫率/磁化率图生成不同的复数数据集（含/不含背景场与残留场）
MacroCreateSusceptibiltyPhantom.m | 示例脚本：如何用弛豫率图和分区参数表生成磁化率幻影
MacroLoopReconstructionsOfPhantoms.m | 脚本：评估不同重建方法的效果（对应论文图7 & 图8）
MacroProcessInvivoData.m | 示例脚本：如何将 data/raw 中的体内数据处理为 QSM 图
TestingResolutionLimitations.m | 脚本：测试分辨率限制
data/ | 目录：以原生分辨率提供的所有输入数据
data/chimodel/Chi.nii.gz | Chi 模型文件（磁化率图）
data/chimodel/ChiModelMIX.nii | Chi 混合模型（QSM Challenge Sim2）
data/chimodel/ChiModelMIX_noCalc.nii | Chi 混合模型（无钙化，QSM Challenge Sim1）
data/chimodel/FinalLabelSuscep2.mat | 最终分割标签与磁化率相关数据（Mat 文件）
data/chimodel/FinalLabelSuscepCalcificationFree.mat | 无钙化情况下的最终标签（Mat 文件）
data/chimodel/paramaters.mat | 生成模型用的参数（Mat 文件）
data/chimodel/paramatersCalcificationFree.mat | 无钙化参数（Mat 文件）
data/chimodel/ProportinalityTermsForSusceptibility.mat | 与磁化率相关的比例项（Mat 文件）
data/maps/ | 目录：相关弛豫率图
data/maps/M0.nii.gz | M0 图（幅值或基线强度图）
data/maps/R1.nii.gz | R1 弛豫率图
data/maps/R2star.nii.gz | R2* 弛豫率图
data/masks/ | 目录：与数字幻影有关的掩模
data/masks/BrainMask.nii.gz | 脑掩模（全脑）
data/masks/BrainMaskBrainExtracted.nii.gz | 已提取脑组织的掩模
data/masks/highgrad.nii.gz | 高级分割/分级掩模
data/masks/SegmentedModel.nii.gz | 分割模型（标注）
data/raw/ | 目录：用于计算弛豫率图的原始数据
data/raw/MP2RAGEME_brain.nii.gz | MP2RAGEME 脑图像（复合文件）
data/raw/MP2RAGEME_INV1.nii | MP2RAGEME 第一反转幅值
data/raw/MP2RAGEME_INV1ph.nii | MP2RAGEME 第一反转相位
data/raw/MP2RAGEME_INV2.nii | MP2RAGEME 第二反转幅值
data/raw/MP2RAGEME_INV2ph.nii | MP2RAGEME 第二反转相位
data/raw/MP2RAGEME_INV2_e2.nii | MP2RAGEME 第二反转第2回波幅值
data/raw/MP2RAGEME_INV2_e2ph.nii | MP2RAGEME 第二反转第2回波相位
data/raw/MP2RAGEME_INV2_e3.nii | MP2RAGEME 第二反转第3回波幅值
data/raw/MP2RAGEME_INV2_e3ph.nii | MP2RAGEME 第二反转第3回波相位
data/raw/MP2RAGEME_INV2_e4.nii | MP2RAGEME 第二反转第4回波幅值
data/raw/MP2RAGEME_INV2_e4ph.nii | MP2RAGEME 第二反转第4回波相位
data/raw/MP2RAGEME_total-field_ppm_head_r2s-header.nii.gz | 总场（ppm）和 r2* 头信息文件
data/raw/sepia/ | 目录：为 QSM 计算处理过的 MP2RAGEME 数据（sepia 工具链）
data/raw/sepia/3T/Derived_HighResSpace/V1.nii.gz | FA 主方向 V1（已配准到高分辨率空间）
data/raw/sepia/3T/Derived_HighResSpace/FA.nii.gz | 分数各向异性 FA（已配准到高分辨率空间）
func/ | 目录：生成幻影与模拟数据的函数
func/CreateOwnRealisticPhantom.m | 函数：创建自定义逼真幻影
func/CreateSimulatedData.m | 函数：根据参数生成模拟数据
func/evaluation/ | 目录：评估脚本
func/utils/ | 目录：工具函数集合
func/utils/nii/ | 子目录：与 NIfTI 相关的实用工具
func/utils/reisert-unring-ddd43da65219/ | 子目录：去环（unringing）实现代码
func/utils/WaveletDenoising/ | 子目录：小波去噪实现
ManuscriptFigures/ | 目录：用于论文图像生成的脚本/数据
ManuscriptFigures/BackgroundFieldRemoval/ | 背景场移除示例（含相位展开）
ManuscriptFigures/BackgroundFieldRemoval/unwrapping/ | 相位展开相关内容
ManuscriptFigures/BackgroundFieldRemovalBrainExtracted/ | 已提取脑组织的背景场移除
ManuscriptFigures/BackgroundFieldRemovalBrainExtracted/unwrapping/ | 相位展开子目录
ManuscriptFigures/BackgroundFieldRemovalHR/ | 高分辨率背景场移除
ManuscriptFigures/BackgroundFieldRemovalHR/unwrapping/ | 相位展开子目录
ManuscriptFigures/BackgroundFieldRemovalHRBrainExtracted/ | 高分辨率且已提取脑组织的背景场移除
ManuscriptFigures/BackgroundFieldRemovalHRBrainExtracted/unwrapping/ | 相位展开子目录
Simdata/ | 目录：不同 MR 协议下的模拟数据集合
Simdata/SimSeqParams.mat | 模拟序列参数（Mat 文件）
Simdata/DGMprotocol/ | 协议：针对深部灰质（Deep Gray Matter）磁化率测量
Simdata/DGMprotocol/SimulationParameters.mat | 仿真参数（Mat 文件）
Simdata/DGMprotocol/SimulatedHR/ | 高分辨率模拟数据（4D 幅值与相位）
Simdata/DGMprotocol/SimulatedHR/Data_magn.nii.gz | 高分辨率模拟的幅值数据（4D）
Simdata/DGMprotocol/SimulatedHR/Data_phase.nii.gz | 高分辨率模拟的相位数据（4D）
Simdata/DGMprotocol/SimulatedHR/Data BrainExtracted_magn.nii.gz | 提取脑组织后的幅值数据
Simdata/DGMprotocol/SimulatedHR/Data BrainExtracted_phase.nii.gz | 提取脑组织后的相位数据
Simdata/DGMprotocol/Simulated_1p0mm/ | 下采样到 1.0 mm 的模拟数据（含 ground truth）
Simdata/DGMprotocol/Simulated_1p0mm/Brain.nii.gz | 脑结构图（下采样）
Simdata/DGMprotocol/Simulated_1p0mm/BrainBrainExtracted.nii.gz | 下采样且提取脑组织的图
Simdata/DGMprotocol/Simulated_1p0mm/Chi_crop.nii.gz | 裁剪后的 Chi（真值）
Simdata/DGMprotocol/Simulated_1p0mm/Chi_cropBrainExtracted.nii.gz | 提取脑组织后的裁剪 Chi（真值）
Simdata/DGMprotocol/Simulated_1p0mm/Chi_interp.nii.gz | 插值后的 Chi（参考/对比用）
Simdata/DGMprotocol/Simulated_1p0mm/Chi_interpBrainExtracted.nii.gz | 插值后并提取脑组织的 Chi
Simdata/DGMprotocol/Simulated_1p0mm/FinalSegment.nii.gz | 最终分割（下采样）
Simdata/DGMprotocol/Simulated_1p0mm/FinalSegmentBrainExtracted.nii.gz | 提取脑组织的最终分割
Simdata/DGMprotocol/Simulated_1p0mm/Data_magn.nii.gz | 下采样模拟的幅值数据
Simdata/DGMprotocol/Simulated_1p0mm/Data_phase.nii.gz | 下采样模拟的相位数据
Simdata/GMWMprotocol/ | 协议：用于区分灰白质（Gray vs White Matter），结构同上
Simdata/ChallengeProtocol/ | 协议：使用 Challenge2.0 模拟协议，子目录结构同上
