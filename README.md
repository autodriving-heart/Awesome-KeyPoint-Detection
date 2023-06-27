## **Awesome**-KeyPoint-Detection

本仓库由[公众号【自动驾驶之心】](https://mp.weixin.qq.com/s?__biz=Mzg2NzUxNTU1OA==&mid=2247542481&idx=1&sn=c6d8609491a128233c3c3b91d68d22a6&chksm=ceb80b18f9cf820e789efd75947633aec9d2f1e8b58c29e5051c05a64b21ae63c244d54886a1&token=11182364&lang=zh_CN#rd) 团队整理，欢迎关注，一览最前沿的技术分享！

自动驾驶之心是国内首个自动驾驶开发者社区！这里有最全面有效的自动驾驶与AI学习路线（感知/定位/融合）和自动驾驶与AI公司内推机会！


## 一、regression-based

Deeppose：Human pose estimation via deep neural networks

## **二、Heatmap-based

#### **Top-Down**方案

Convolutional Pose Machines. CVPR 2016.

Stacked Hourglass Networks for Human Pose Estimation. ECCV 2016

Towards accurate multi-person pose estimation in the wild. CVPR 2017

A coarse-ﬁne network for keypoint localization. ICCV 2017. 

Cascaded pyramid network for multi-person pose estimation. CVPR 2018.

Simple baselines for human pose estimation and tracking.  ECCV 2018

Deep high-resolution representation learning for human pose estimation. CVPR 2019.

Poseﬁx: Model-agnostic general human pose reﬁnement network. CVPR 2019

Distribution-Aware Coordinate Representation for Human Pose Estimation. CVPR 2020.

The Devils is in the Details: Delving into Unbiased Data Processing for human pose estimation. CVPR 2020.

#### Bottom-up方案

DeepCut Joint subset partition and labeling for multi person pose estimation. CVPR 2016

Deepcut : A deeper, stronger, and faster multi-person pose estimation model. ECCV 2016

OpenPose：Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields. CVPR 2017

Pifpaf: Composite ﬁelds for human pose estimation. CVPR 2019

Single-stage multi-person pose machines. ICCV 2019

Higherhrnet: Scale-aware representation learning for bottom-up human pose estimation. CVPR 2020

Rethinking the Heatmap Regression for Bottom-up Human Pose Estimation. CVPR 2021.

## **三、 Keypoint Problem

**1、目标遮挡、重叠丢点问题**

在训练阶段，采用Grid Mak刻意制造遮挡点优化整体拓扑结构的稳定；

bottom-up方案还存在丢点和点匹配异常问题，对于点数要求严格的情况，可以优先采用top-down和回归方案。

**2、光照影响**

过亮过暗问题，需要在训练阶段增加数据增强