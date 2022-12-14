# 摘要

我们提出了ROCA1，一种新颖的端到端方法，从形状数据库检索3D CAD模型并将其对齐到单个输入图像。这使得从2D RGB观测中观察到的场景具有3D感知能力，其特点是轻量级、紧凑、干净的CAD表示。我们方法的核心是基于密集2D-3D对象对应和Procrustes对齐的可微对齐优化。因此，ROCA可以提供一个健壮的CAD对齐，同时通过利用2D-3D对应关系来学习几何相似的CAD模型，从而通知CAD检索。在具有挑战性的、来自ScanNet的真实图像上进行的实验表明，ROCA在现有技术水平上有显著提高，检索感知CAD对齐精度从9.5%提高到17.6%。

# 介绍

我们提出了一种用于CAD模型对RGB图像对齐的端到端体系结构:

一种新的可微位姿优化，使几何感知的2d - 3d CAD对RGB图像对齐，

通过利用密集的物体姿态对应关系和代理CAD完成目标来改进CAD检索，以通知被检测物体和CAD模型之间的联合嵌入空间的构造，

每个图像的交互运行时间为53毫秒，便于在实时应用程序中使用。