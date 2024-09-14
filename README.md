# GenMapping
GenMapping: Unleashing the Potential of Inverse Perspective Mapping for Robust Online HD Map Construction

## Motivation
<div align=center>
<img src="https://github.com/lynn-yu/GenMapping/blob/main/motivation.png" width="50%" >
</div>

## Framework
<div align=center>
<img src="https://github.com/lynn-yu/GenMapping/blob/main/frame.png" >
</div>

### Abstract
Online High-Definition (HD) maps have emerged as the preferred option for autonomous driving, overshadowing the counterpart offline HD maps due to flexible update capability and lower maintenance costs. However, contemporary online HD map models embed parameters of visual sensors into training, resulting in a significant decrease in generalization performance when applied to visual sensors with different parameters. Inspired by the inherent potential of Inverse Perspective Mapping (IPM), where camera parameters are decoupled from the training process, we have designed a universal map generation framework, GenMapping. The framework is established with a triadic synergy architecture, including principal and dual auxiliary branches. When faced with a coarse road image with local distortion translated via IPM, the principal branch learns robust global features under the state space models. The two auxiliary branches are a dense perspective branch and a sparse prior branch. The former exploits the correlation information between static and moving objects, whereas the latter introduces the prior knowledge of OpenStreetMap (OSM). The triple-enhanced merging module is crafted to synergistically integrate the unique spatial features from all three branches. To further improve generalization capabilities, a Cross-View Map Learning (CVML) scheme is leveraged to realize joint learning within the common space. Additionally, a Bidirectional Data Augmentation (BiDA) module is introduced to mitigate reliance on datasets concurrently. A thorough array of experimental results shows that the proposed model surpasses current state-of-the-art methods in both semantic mapping and vectorized mapping, while also maintaining a rapid inference speed. Moreover, in cross-dataset experiments, the generalization of semantic mapping is improved by 17.3% in mIoU, while vectorized mapping is improved by 12.1% in mAP. 

### Update
2024.9 Init repository.
