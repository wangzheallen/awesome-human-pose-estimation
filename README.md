# Awesome Human Pose Estimation [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

<p align="center">
  <img src="diagram_2.png" width=700>
</p>


A collection of resources on human pose related problem: mainly focus on human pose estimation, and will include mesh representation, flow calculation, kinematics, or maybe sequence learning.

## Why awesome human pose estimation?

This is a collection of papers and resources I curated when learning the ropes in Human Pose estimation. And This is a fork from https://github.com/cbsudux/awesome-human-pose-estimation (thanks for cbsudux) and customized for personal study and sharing. I will be continuously updating this list with the latest papers and resources. If you want some theory on Human Pose Estimation, check out [Pose Related_Human_Knowledge](https://github.com/wangzheallen/pose_related_human_knowledge/blob/master/README.md)

## Related Pages:
https://github.com/xinghaochen/awesome-hand-pose-estimation
https://github.com/1adrianb/face-alignment
## Contributing

If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/wangzheallen/awesome-human-pose-estimation/pulls)

Feedback and contributions are welcome!

## Table of Contents
- [Basics](#basics)
- [Papers](#papers)
  - [2D Pose estimation](#2d-pose-estimation)
  - [3D Pose estimation](#3d-pose-estimation)
  - [Person generation](#person-generation)
  - [Video pose](#video-pose)
  - [Real-time Pose estimation](#real-time-pose-estimation)
  - [Hand-Face Pose which is inspiring](#Hand-Face-landmark)
- [Datasets](#datasets)
- [Workshops](#workshops) 
- [Blog posts](#blogposts)
- [Popular implementations](#popular-implementations)
  - [PyTorch](#pytorch)
  - [TensorFlow](#tensorflow)
  - [Torch](#Torch)
  - [Others](#others)

## Basics
- [pose_related_human_knowledge](https://github.com/wangzheallen/pose_related_human_knowledge)

## Papers

### 2D Pose estimation
- [Learning Human Pose Estimation Features with Convolutional Networks](https://arxiv.org/pdf/1312.7302.pdf) - Jain, A., Tompson, J., Andriluka, M., Taylor, G.W., & Bregler, C. (ICLR 2013) 
- [DeepPose: Human Pose Estimation via Deep Neural Networks](https://arxiv.org/pdf/1312.4659.pdf) - Toshev, A., & Szegedy, C. (CVPR 2014)
- [Joint Training of a Convolutional Network and a Graphical Model for Human Pose Estimation](https://arxiv.org/pdf/1406.2984.pdf) - [[CODE]](https://github.com/max-andr/joint-cnn-mrf) - Tompson, J., Jain, A., LeCun, Y., & Bregler, C. (NIPS 2014) 
- [MoDeep: A Deep Learning Framework Using Motion Features for Human Pose Estimation](https://arxiv.org/pdf/1409.7963.pdf) - Jain, A., Tompson, J., LeCun, Y., & Bregler, C. (ACCV 2014)
- [Efficient Object Localization Using Convolutional Networks](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.858.5872&rep=rep1&type=pdf) - Tompson, J., Goroshin, R., Jain, A., LeCun, Y., & Bregler, C (CVPR 2015)
- [Flowing ConvNets for Human Pose Estimation in Videos](https://arxiv.org/pdf/1506.02897.pdf) - [[CODE]](https://github.com/tpfister/caffe-heatmap) - Pfister, T., Charles, J., & Zisserman, A. (ICCV 2015)
- [Convolutional Pose Machines](https://arxiv.org/pdf/1602.00134.pdf) - [[CODE]](https://github.com/shihenw/convolutional-pose-machines-release) - Wei, S., Ramakrishna, V., Kanade, T., & Sheikh, Y. (CVPR 2016)
- [Human Pose Estimation with Iterative Error Feedback](https://arxiv.org/pdf/1507.06550.pdf)- [[CODE]](https://github.com/pulkitag/ief) Carreira, J., Agrawal, P., Fragkiadaki, K., & Malik, J. (CVPR 2016) 
- [DeepCut: Joint Subset Partition and Labeling for Multi Person Pose Estimation](https://arxiv.org/pdf/1511.06645.pdf) - [[CODE]](https://github.com/eldar/deepcut) - Pishchulin, L., Insafutdinov, E., Tang, S., Andres, B., Andriluka, M., Gehler, P.V., & Schiele, B. (CVPR 2016)
- [DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model](https://arxiv.org/pdf/1605.03170.pdf) - [[CODE1]](https://github.com/eldar/deepcut-cnn)[[CODE2]](https://github.com/eldar/pose-tensorflow) - Insafutdinov, E., Pishchulin, L., Andres, B., Andriluka, M., & Schiele, B. (ECCV 2016)
- [Stacked Hourglass Networks for Human Pose Estimation](https://arxiv.org/pdf/1603.06937.pdf) - [[CODE]](https://github.com/umich-vl/pose-hg-demo) - Newell, A., Yang, K., & Deng, J. (ECCV 2016) 
- [Multi-context Attention for Human Pose Estimation](https://arxiv.org/pdf/1702.07432.pdf) - [[CODE]](https://github.com/bearpaw/pose-attention) - Chu, X., Yang, W., Ouyang, W., Ma, C., Yuille, A.L., & Wang, X. (CVPR 2017)
- [Towards Accurate Multi-person Pose Estimation in the Wild](https://arxiv.org/pdf/1701.01779.pdf) - [[CODE]](https://github.com/hackiey/keypoints) - Papandreou, G., Zhu, T., Kanazawa, N., Toshev, A., Tompson, J., Bregler, C., & Murphy, K.P. (CVPR 2017) 
- [Realtime Multi-person 2D Pose Estimation Using Part Affinity Fields](https://arxiv.org/pdf/1611.08050.pdf) - [[CODE]](https://github.com/ZheC/Realtime_Multi-Person_Pose_Estimation) - Cao, Z., Simon, T., Wei, S., & Sheikh, Y. (CVPR 2017) 
- [Learning Feature Pyramids for Human Pose Estimation](https://arxiv.org/pdf/1708.01101.pdf) - [[CODE]](https://github.com/bearpaw/PyraNet) - Yang, W., Li, S., Ouyang, W., Li, H., & Wang, X. (ICCV 2017)
- [Human Pose Estimation Using Global and Local Normalization](https://arxiv.org/pdf/1709.07220.pdf) - Sun, K., Lan, C., Xing, J., Zeng, W., Liu, D., & Wang, J. (ICCV 2017) 
- [Adversarial PoseNet: A Structure-Aware Convolutional Network for Human Pose Estimation](https://arxiv.org/pdf/1705.00389.pdf) - Chen, Y., Shen, C., Wei, X., Liu, L., & Yang, J. (ICCV 2017)
- [RMPE: Regional Multi-person Pose Estimation](https://arxiv.org/pdf/1612.00137.pdf) - [[CODE1]](https://github.com/Fang-Haoshu/RMPE)[[CODE2]](https://github.com/MVIG-SJTU/AlphaPose) - Fang, H., Xie, S., & Lu, C. (ICCV 2017)
- [Self Adversarial Training for Human Pose Estimation](https://arxiv.org/pdf/1707.02439.pdf) - [[CODE1]](https://github.com/dongzhuoyao/jessiechouuu-adversarial-pose)[[CODE2]](https://github.com/roytseng-tw/adversarial-pose-pytorch) - Chou, C., Chien, J., & Chen, H. (ArXiv 2017)
- [Recurrent Human Pose Estimation](https://arxiv.org/pdf/1605.02914.pdf) - [[CODE]](https://github.com/ox-vgg/keypoint_detection) - Belagiannis, V., & Zisserman, A. (FG 2017)
- [Knowledge-Guided Deep Fractal Neural Networks for Human Pose Estimation](https://arxiv.org/pdf/1705.02407.pdf) - [[CODE]](https://github.com/Guanghan/GNet-pose) Ning, G., Zhang, Z., & He, Z. (IEEE Transactions on Multimedia 2018)
- [Human Pose Estimation with Parsing Induced Learner](http://openaccess.thecvf.com/content_cvpr_2018/papers/Nie_Human_Pose_Estimation_CVPR_2018_paper.pdf)- Xuecheng Nie, Jiashi Feng, Yiming Zuo, Shuicheng Yan (CVPR 2018)
- [LSTM Pose Machines](https://arxiv.org/pdf/1712.06316.pdf) - [[CODE]](https://github.com/lawy623/LSTM_Pose_Machines) - Yue Luo, Jimmy Ren, Zhouxia Wang, Wenxiu Sun, Jinshan Pan, Jianbo Liu, Jiahao Pang, Liang Lin (CVPR 2018)
- [Simple Baselines for Human Pose Estimation
and Tracking](http://openaccess.thecvf.com/content_ECCV_2018/papers/Bin_Xiao_Simple_Baselines_for_ECCV_2018_paper.pdf) - [[CODE]](https://github.com/Microsoft/human-pose-estimation.pytorch) - Bin, Xiao, Haiping Wu, Yichen Wei (ECCV 2018)
- [Multi-Scale Structure-Aware Network for Human Pose Estimation](http://openaccess.thecvf.com/content_ECCV_2018/papers/Lipeng_Ke_Multi-Scale_Structure-Aware_Network_ECCV_2018_paper.pdf) - Lipeng Ke, Ming-Ching Chang, Honggang Qi, Siwei Lyu (ECCV 2018)
- [Deeply Learned Compositional Models for Human Pose Estimation](http://openaccess.thecvf.com/content_ECCV_2018/papers/Wei_Tang_Deeply_Learned_Compositional_ECCV_2018_paper.pdf) - [[CODE]](http://www.ece.northwestern.edu/~wtt450/project/ECCV18_DLCM/) - Wei Tang, Pei Yu, Ying Wu (ECCV 2018)

### 3D Pose estimation

- [3D Human Pose Estimation from Monocular Images with Deep Convolutional Neural Network](http://visal.cs.cityu.edu.hk/static/pubs/conf/accv14-3dposecnn.pdf) - Li, S., & Chan, A.B. (ACCV 2014)
- [Sparseness Meets Deepness: 3D Human Pose Estimation from Monocular Video](http://arxiv.org/abs/1511.09439) - [[CODE]](https://github.com/daniilidis-group/monocap) - X. Zhou, M. Zhu, G. Pavlakos, S. Leonardos, K.G. Derpanis, K. Daniilidis. (CVPR 2016)
- [Structured Prediction of 3D Human Pose with Deep Neural Networks](https://arxiv.org/pdf/1605.05180.pdf) - Tekin, B., Katircioglu, I., Salzmann, M., Lepetit, V., & Fua, P. (BMVC 2016)
- [VNect: Real-time 3D Human Pose Estimation with a Single RGB Camera](http://gvv.mpi-inf.mpg.de/projects/VNect/content/VNect_SIGGRAPH2017.pdf) - [[CODE]](https://github.com/timctho/VNect-tensorflow) - Mehta, Dushyant et al. (SIGGRAPH 2017)
- [Recurrent 3D Pose Sequence Machines](https://arxiv.org/pdf/1707.09695.pdf) - Lin, M., Lin, L., Liang, X., Wang, K., & Cheng, H. (CVPR 2017)
- [Lifting from the Deep: Convolutional 3D Pose Estimation from a Single Image](https://arxiv.org/pdf/1701.00295.pdf) - Tomè, D., Russell, C., & Agapito, L. (CVPR 2017)
- [Coarse-to-Fine Volumetric Prediction for Single-Image 3D Human Pose](https://arxiv.org/pdf/1611.07828.pdf) - [[CODE]](https://github.com/geopavlakos/c2f-vol-demo) - Pavlakos, G., Zhou, X., Derpanis, K.G., & Daniilidis, K. (CVPR 2017)
- [LCR-Net: Localization-Classification-Regression for Human Pose](https://www.researchgate.net/publication/315867122_LCR-Net_Localization-Classification-Regression_for_Human_Pose) - [[CODE]](https://thoth.inrialpes.fr/src/LCR-Net/) - Grégory Rogez, Philippe Weinzaepfel, Cordelia Schmid. (CVPR 2017)
- [Harvesting Multiple Views for Marker-less 3D Human Pose Annotations](https://www.seas.upenn.edu/~pavlakos/projects/harvesting/files/harvesting.pdf) - [[CODE]](https://github.com/geopavlakos/harvesting/) - G. Pavlakos, X. Zhou, K. Derpanis, K. Daniilidis.  (CVPR 2017)
- [Towards 3D Human Pose Estimation in the Wild: a Weakly-supervised Approach](https://arxiv.org/pdf/1704.02447.pdf) - [[CODE]](https://github.com/xingyizhou/Pytorch-pose-hg-3d) - Zhou, X., Huang, Q., Sun, X., Xue, X., & Wei, Y. (ICCV 2017)
- [A Simple Yet Effective Baseline for 3d Human Pose Estimation](https://arxiv.org/pdf/1705.03098.pdf) - [[CODE]](https://github.com/weigq/3d_pose_baseline_pytorch) - Martinez, J., Hossain, R., Romero, J., & Little, J.J. (ICCV 2017)
- [Sparse Representation for 3D Shape Estimation: A Convex Relaxation Approach](http://arxiv.org/abs/1509.04309) - [[CODE]](http://www.cad.zju.edu.cn/home/xzhou/code/shapeconvex.zip) - X. Zhou, M. Zhu, S. Leonardos, K. Daniilidis. (PAMI 2017)
- [Compositional Human Pose Regression](https://arxiv.org/pdf/1704.00159.pdf) - Sun, X., Shang, J., Liang, S., & Wei, Y. (ICCV 2017)
- [Monocular 3D Human Pose Estimation In The Wild Using Improved CNN Supervision](http://gvv.mpi-inf.mpg.de/3dhp-dataset/) - Mehta, D., Rhodin, H., Casas, D., Fua, P., Sotnychenko, O., Xu, W., & Theobalt, C. (3DV 2017)
- [3D Human Pose Estimation in the Wild by Adversarial Learning](https://arxiv.org/pdf/1803.09722.pdf) - Yang, W., Ouyang, W., Wang, X., Ren, J.S., Li, H., & Wang, X. (CVPR 2018)
- [Ordinal Depth Supervision for 3D Human Pose Estimation](https://arxiv.org/pdf/1805.04095.pdf) - [[CODE]](https://github.com/geopavlakos/ordinal-pose3d/) - G. Pavlakos, X. Zhou, K. Daniilidis. (CVPR 2018)
- [DRPose3D: Depth Ranking in 3D Human Pose Estimation](https://arxiv.org/pdf/1805.08973.pdf) - Wang, M., Chen, X., Liu, W., Qian, C., Lin, L., & Ma, L. (IJCAI 2018)
- [Human Motion Capture Using a Drone](https://arxiv.org/abs/1804.06112) - X. Zhou, S. Liu, G. Pavlakos, V.J. Kumar, K. Daniilidis. (ICRA 2018)
- [End-to-end Recovery of Human Shape and Pose](https://arxiv.org/pdf/1712.06584.pdf) - [[CODE]](https://github.com/akanazawa/hmr) - Kanazawa, A., Black, M.J., Jacobs, D.W., & Malik, J. (CVPR 2018)
- [Learning to Estimate 3D Human Pose and Shape from a Single Color Image](http://openaccess.thecvf.com/content_cvpr_2018/papers/Pavlakos_Learning_to_Estimate_CVPR_2018_paper.pdf) - Pavlakos, G., Zhu, L., Zhou, X., & Daniilidis, K. (CVPR 2018)
- [Dense Human Pose Estimation In The Wild](https://arxiv.org/pdf/1802.00434.pdf) - [[CODE]](https://github.com/facebookresearch/Densepose) - Guler, R.A., Neverova, N., & Kokkinos, I. (CVPR 2018)
- [Neural Body Fitting: Unifying Deep Learning and Model-Based Human Pose and Shape Estimation](https://arxiv.org/pdf/1808.05942.pdf) - [[CODE]](https://github.com/mohomran/neural_body_fitting) - Omran, Mohamed and Lassner, Christoph and Pons-Moll, Gerard and Gehler, Peter V. and Schiele, Bernt (3DV 2018)
- [Learning 3D Human Pose from Structure and Motion](http://openaccess.thecvf.com/content_ECCV_2018/papers/Rishabh_Dabral_Learning_3D_Human_ECCV_2018_paper.pdf) - Dabral, R., Mundhada, A., Kusupati, U., Afaque, S., Sharma, A., & Jain, A. (ECCV 2018)
- [Integral Human Pose Regression](https://arxiv.org/pdf/1711.08229.pdf) - [[CODE]](https://github.com/JimmySuen/integral-human-pose) - Sun, X., Xiao, B., Liang, S., & Wei, Y. (ECCV 2018)
- [Dense Pose Transfer](https://arxiv.org/pdf/1809.01995.pdf) - Neverova, N., Guler, R.A., & Kokkinos, I. (ECCV 2018)
- [Unsupervised Geometry-Aware Representation for 3D Human Pose Estimation](http://openaccess.thecvf.com/content_ECCV_2018/papers/Helge_Rhodin_Unsupervised_Geometry-Aware_Representation_ECCV_2018_paper.pdf) - [[CODE]](https://github.com/hrhodin/UnsupervisedGeometryAwareRepresentationLearning) - Rhodin, H., Salzmann, M., & Fua, P. (ECCV 2018)
- [BodyNet: Volumetric Inference of 3D Human Body Shapes](https://arxiv.org/pdf/1804.04875v3.pdf) - [[CODE]](https://github.com/gulvarol/bodynet) - Varol, G., Ceylan, D., Russell, B., Yang, J., Yumer, E., Laptev, I., & Schmid, C. (ECCV 2018)
- [Monocap: Monocular human motion capture using a CNN coupled with a geometric prior](https://arxiv.org/abs/1701.02354) - [[CODE]](https://github.com/daniilidis-group/monocap) - X. Zhou, M. Zhu, G. Pavlakos, S. Leonardos, K.G. Derpanis, K. Daniilidis. (TPAMI 2018)


### Person generation
- [Binge Watching: Scaling Affordance Learning from Sitcoms. ](https://www.cs.cmu.edu/~xiaolonw/papers/CVPR_2017_VAE_affordance.pdf) - [[CODE]](https://www.cs.cmu.edu/~xiaolonw/affordance.html) - Xiaolong Wang*, Rohit Girdhar*, and Abhinav Gupta. (CVPR 2017)
- [Pose Guided Person Image Generation](https://arxiv.org/pdf/1705.09368.pdf) - [[CODE]](https://github.com/charliememory/Pose-Guided-Person-Image-Generation) - Ma, L., Jia, X., Sun, Q., Schiele, B., Tuytelaars, T., & Gool, L.V. (NIPS 2017)
- [A Generative Model of People in Clothing](https://arxiv.org/pdf/1705.04098.pdf) - Lassner, C., Pons-Moll, G., & Gehler, P.V. (ICCV 2017)
- [Synthesizing Images of Humans in Unseen Poses](http://openaccess.thecvf.com/content_cvpr_2018/papers/Balakrishnan_Synthesizing_Images_of_CVPR_2018_paper.pdf) - [[CODE]](https://github.com/balakg/posewarp-cvpr2018) - Guha Balakrishnan, Amy Zhao, Adrian V. Dalca, Fredo Durand, John Guttag. (CVPR 2018)
- [A Variational U-Net for Conditional Appearance and Shape Generation](https://compvis.github.io/vunet/images/vunet.pdf) - [[CODE]](https://github.com/CompVis/vunet) - Patrick Esser, Ekaterina Sutter, Björn Ommer. (CVPR 2018)
- [Deformable GANs for Pose-based Human Image Generation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Siarohin_Deformable_GANs_for_CVPR_2018_paper.pdf) - [[CODE]](https://github.com/AliaksandrSiarohin/pose-gan) - Siarohin, A., Sangineto, E., Lathuilière, S., & Sebe, N. (CVPR 2018)
- [Dense Pose Transfer](https://arxiv.org/pdf/1809.01995.pdf) - Neverova, N., Guler, R.A., & Kokkinos, I. (ECCV 2018)
- [MT-VAE: Learning Motion Transformations to Generate Multimodal Human Dynamics](https://arxiv.org/abs/1808.04545) - Xinchen Yan, Akash Rastogi, Ruben Villegas, Kalyan Sunkavalli, Eli Shechtman, Sunil Hadap, Ersin Yumer, Honglak Lee (ECCV 2018)
- [ Everybody Dance Now](https://carolineec.github.io/everybody_dance_now/) - Caroline Chan, Shiry Ginosar, Tinghui Zhou, Alexei A. Efros  (Arxiv 2018)

### Video pose
- [Pose from Flow and Flow from Pose](http://www.cis.upenn.edu/~jshi/papers/CVPR2013_posefromflow.pdf) - Katerina Fragkiadaki, Han Hu and Jianbo Shi . (CVPR 2013)
- [Personalizing Human Video Pose Estimation](https://arxiv.org/pdf/1511.06676.pdf) - James Charles, Tomas Pfister, Derek Magee, David Hogg, Andrew Zisserman . (CVPR 2016)
- [Thin-Slicing Network: A Deep Structured Model for Pose Estimation in Videos](https://arxiv.org/pdf/1703.10898.pdf) - Jie Song, Limin Wang, Luc Van Gool, Otmar Hilliges. (CVPR 2017)
- [Deep Multitask Architecture for Integrated 2D and 3D Human Sensing,](http://openaccess.thecvf.com/content_cvpr_2017/papers/Popa_Deep_Multitask_Architecture_CVPR_2017_paper.pdf) - [[CODE]](https://github.com/alinionutpopa/dmhs) - Alin-Ionut Popa and Mihai Zanfir and Cristian Sminchisescu. (CVPR 2017)
- [Rpan: An end-to-end recurrent pose-attention network for action recognition in videos](http://openaccess.thecvf.com/content_ICCV_2017/papers/Du_RPAN_An_End-To-End_ICCV_2017_paper.pdf) - Wenbin Du, Yali Wang, Yu Qiao. (ICCV 2017)
- [Self-supervised Learning of Motion Capture](http://papers.nips.cc/paper/7108-self-supervised-learning-of-motion-capture.pdf) - [[CODE]](https://sites.google.com/view/selfsupervisedlearningofmotion/) - Hsiao-Yu Fish Tung,  Hsiao-Wei Tung,  Ersin Yumer,  Katerina Fragkiadaki. (NIPS 2017)
- [Detect-and-Track: Efficient Pose Estimation in Videos,](https://arxiv.org/abs/1712.09184) - [[CODE]](https://github.com/facebookresearch/DetectAndTrack/) - Rohit Girdhar, Georgia Gkioxari, Lorenzo Torresani, Manohar Paluri and Du Tran. (CVPR 2018)
- [Neural Kinematic Networks for Unsupervised Motion Retargeting,](https://eng.ucmerced.edu/people/jyang44/papers/cvpr2018_NeuralKinematicNetworks_camera_ready.pdf) - [[CODE]](https://github.com/rubenvillegas/cvpr2018nkn) - Ruben Villegas, Jimei Yang, Duygu Ceylan, Honglak Lee. (CVPR 2018)
- [Spatial Temporal Graph Convolutional Networks for Skeleton-Based Action Recognition,](https://arxiv.org/pdf/1801.07455.pdf) - [[CODE]](https://github.com/yysijie/st-gcn) - Sijie Yan, Yuanjun Xiong, and Dahua Lin. (AAAI 2018)
- [QuaterNet: A Quaternion-based Recurrent Model for Human Motion](https://arxiv.org/abs/1805.06485) - [[CODE]](https://github.com/facebookresearch/QuaterNet) - Dario Pavllo, David Grangier, and Michael Auli. (BMVC 2018)
- [Simple Baselines for Human Pose Estimation and Tracking](https://arxiv.org/pdf/1804.06208.pdf) - [[CODE]](https://github.com/Microsoft/human-pose-estimation.pytorch) - Bin Xiao, Haiping Wu, Yichen Wei. (ECCV 2018)
- [Learning 3D Human Pose from Structure and Motion](http://openaccess.thecvf.com/content_ECCV_2018/papers/Rishabh_Dabral_Learning_3D_Human_ECCV_2018_paper.pdf) - Dabral, R., Mundhada, A., Kusupati, U., Afaque, S., Sharma, A., & Jain, A. (ECCV 2018)
- [SFV: Reinforcement Learning of Physical Skills from Videos](https://xbpeng.github.io/projects/SFV/2018_TOG_SFV.pdf) - Xue Bin Peng, Angjoo Kanazawa, Jitendra Malik, Pieter Abbeel, Sergey Levine. (ACM SIGGRAPH Asia 2018)

### Real-time pose estimation


- [Realtime Multi-person 2D Pose Estimation Using Part Affinity Fields](https://arxiv.org/pdf/1611.08050.pdf) - [[CODE]](https://github.com/ZheC/Realtime_Multi-Person_Pose_Estimation) - Cao, Z., Simon, T., Wei, S., & Sheikh, Y. (CVPR 2017) 
- [VNect: Real-time 3D Human Pose Estimation with a Single RGB Camera](http://gvv.mpi-inf.mpg.de/projects/VNect/content/VNect_SIGGRAPH2017.pdf) - [[CODE]](https://github.com/timctho/VNect-tensorflow) - Mehta, Dushyant et al. (SIGGRAPH 2017)
- [RMPE: Regional Multi-person Pose Estimation](https://arxiv.org/pdf/1612.00137.pdf) - [[CODE1]](https://github.com/Fang-Haoshu/RMPE)[[CODE2]](https://github.com/MVIG-SJTU/AlphaPose) - Fang, H., Xie, S., & Lu, C. (ICCV 2017)
- [Dense Human Pose Estimation In The Wild](https://arxiv.org/pdf/1802.00434.pdf) - [[CODE]](https://github.com/facebookresearch/Densepose) - Guler, R.A., Neverova, N., & Kokkinos, I. (CVPR 2018)
- [MultiPoseNet: Fast Multi-Person Pose Estimation using Pose Residual Network](https://arxiv.org/pdf/1807.04067.pdf) - [[CODE]](https://github.com/mkocabas/pose-residual-network) - Guler, R.A., Neverova, N., & Kokkinos, I. (ECCV 2018)

### Hand-Face-landmark
- [Hand PointNet: 3D Hand Pose Estimation Using Point Sets](http://openaccess.thecvf.com/content_cvpr_2018/papers/Ge_Hand_PointNet_3D_CVPR_2018_paper.pdf)  - Liuhao Ge, Yujun Cai, Junwu Weng, Junsong Yuan (CVPR 2018)
- [Real-Time Rotation-Invariant Face Detection with Progressive Calibration Networks](https://arxiv.org/abs/1804.06039)  - [[CODE]](https://github.com/Jack-CV/PCN-FaceDetection-FaceAlignment) - Xuepeng Shi, Shiguang Shan, Meina Kan, Shuzhe Wu, Xilin Chen (CVPR 2018)




## Datasets
### 2D
- [MPII Human Pose Dataset](http://human-pose.mpi-inf.mpg.de/)
- [LSP](http://sam.johnson.io/research/lsp.html)
- [FLIC](https://bensapp.github.io/flic-dataset.html)
- [FLIC-plus](https://cims.nyu.edu/~tompson/flic_plus.htm)

### 3D
- [Human3.6M](http://vision.imar.ro/human3.6m/description.php)
- [HumanEva](http://humaneva.is.tue.mpg.de/)
- [MPI-INF-3DHP](http://gvv.mpi-inf.mpg.de/3dhp-dataset/)
- [Unite The People](http://files.is.tuebingen.mpg.de/classner/up/)

### Meshes
- [Surreal](https://github.com/gulvarol/surreal)

## Workshops
- [POSETRACK-ECCV](https://posetrack.net/workshops/eccv2018/)
- [3D HUMANS-CVPR 2018](https://project.inria.fr/humans2018/)


## Blog posts
- [Real-time Human Pose Estimation in the Browser with TensorFlow.js](https://medium.com/tensorflow/real-time-human-pose-estimation-in-the-browser-with-tensorflow-js-7dd0bc881cd5)
- [Deep learning for human pose estimation](https://www.slideshare.net/plutoyang/mmlab-seminar-2016-deep-learning-for-human-pose-estimation)
- [Deep Learning based Human Pose Estimation using OpenCV ( C++ / Python )](https://www.learnopencv.com/deep-learning-based-human-pose-estimation-using-opencv-cpp-python/)

## Popular implementations


### PyTorch
- [pytorch-pose-hg-3d](https://github.com/xingyizhou/Pytorch-pose-hg-3d)
- [pytorch_Realtime_Multi-Person_Pose_Estimation](https://github.com/tensorboy/pytorch_Realtime_Multi-Person_Pose_Estimation)
- [AlphaPose](https://github.com/MVIG-SJTU/AlphaPose/tree/pytorch)
- [pytorch-pose](https://github.com/bearpaw/pytorch-pose)
- [human-pose-estimation.pytorch](https://github.com/Microsoft/human-pose-estimation.pytorch)

### TensorFlow

- [tf-pose-estimation](https://github.com/ildoonet/tf-pose-estimation)
- [pose-tensorflow](https://github.com/eldar/pose-tensorflow)

### Torch

- [pose-hg-train](https://github.com/umich-vl/pose-hg-train)
- [pose-hg-demo](https://github.com/umich-vl/pose-hg-demo)

### Others

- [openpose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
- [DensePose](https://github.com/facebookresearch/DensePose)

## Todo

- [x] Add basics
- [ ] Add a SOTA ranking
- [ ] Pose forecasting

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.










