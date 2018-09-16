# LADCF - No 1 Algorithm on the public dataset of [VOT2018](http://www.votchallenge.net/vot2018/)
Codes of 'Learning Adaptive Discriminative Correlation Filters (LADCF) via Temporal Consistency preserving Spatial Feature Selection for Robust Visual Tracking' for VOT2018

## [Download the Paper](https://www.researchgate.net/publication/326696472_Learning_Adaptive_Discriminative_Correlation_Filters_via_Temporal_Consistency_Preserving_Spatial_Feature_Selection_for_Robust_Visual_Tracking)
>@article{xu2018learning,
  title={Learning Adaptive Discriminative Correlation Filters via Temporal Consistency Preserving Spatial Feature Selection for Robust Visual Tracking},
  author={Xu, Tianyang and Feng, Zhen-Hua and Wu, Xiao-Jun and Kittler, Josef},
  journal={arXiv preprint arXiv:1807.11348},
  year={2018}}

### Instruction for LADCF Tracker for VOT2018:
Learning Adaptive Discriminative Correlation Filter on Low-dimensional Manifold (LADCF) utilises adaptive spatial regularizer to train low-dimensional discriminative correlation filters. We follow a single-frame learning and updating strategy: the filters are learned after tracking stage and then updated using a fixed rate [1]. We use HOG [2], CN [3], and ResNet-50 [4] as our features.  For deep features, we augment the training data using blur (2 gaussian filters), rotation (-30, -20, -10, 10, 20, 30) and flip (horizontal) [5]. Code modules refer to ECO [6] in feature extraction.

#### Installation:
Run install.m file to compile the libraries.
Copy the tracker_LADCF.m to the vot-workspace. (replace #LOCATION with the path of this folder)

#### Dependencies:
- [MatConvNet](http://www.vlfeat.org/matconvnet/)  
- [PDollar Toolbox](https://pdollar.github.io/toolbox)
- mtimesx (https://github.com/martin-danelljan/ECO/tree/master/external_libs/mtimesx)
- mexResize (https://github.com/martin-danelljan/ECO/tree/master/external_libs/mexResize) 

#### Operating system:
Ubuntu 14.04 LTS, Matlab R2016a, CPU Intel(R) Xeon(R) E5-2643 

#### References:
- [1] Henriques, João F., et al. "High-speed tracking with kernelized correlation filters." 
IEEE Transactions on Pattern Analysis and Machine Intelligence 37.3 (2015): 583-596.
- [2] Dalal, Navneet, and Bill Triggs. "Histograms of oriented gradients for human detection." 
Computer Vision and Pattern Recognition, 2005. CVPR 2005. 
- [3] Van De Weijer, Joost, et al. "Learning color names for real-world applications." 
IEEE Transactions on Image Processing 18.7 (2009): 1512-1523.
- [4] He, Kaiming, et al. "Deep residual learning for image recognition." 
Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.
- [5] Bhat, Goutam, Joakim Johnander, Martin Danelljan, Fahad Shahbaz Khan, and 
Michael Felsberg. "Unveiling the Power of Deep Tracking." arXiv preprint arXiv:1804.06833 (2018).
- [6] Danelljan, Martin, et al. "Eco: Efficient convolution operators for tracking." 
Proceedings of the 2017 IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2017.

