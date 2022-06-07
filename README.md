[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/dino-detr-with-improved-denoising-anchor-1/object-detection-on-coco-minival)](https://paperswithcode.com/sota/object-detection-on-coco-minival?p=dino-detr-with-improved-denoising-anchor-1)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/dino-detr-with-improved-denoising-anchor-1/object-detection-on-coco)](https://paperswithcode.com/sota/object-detection-on-coco?p=dino-detr-with-improved-denoising-anchor-1)

This is the official implementation of the paper "[DINO: DETR with Improved DeNoising Anchor Boxes for End-to-End Object Detection](https://arxiv.org/abs/2203.03605)".

Authors: [Hao Zhang](https://scholar.google.com/citations?user=B8hPxMQAAAAJ&hl=zh-CN)\*, [Feng Li](https://fengli-ust.github.io/)\*, [Shilong Liu](https://www.lsl.zone/)\*, [Lei Zhang](https://www.leizhang.org/), [Hang Su](https://www.suhangss.me/), [Jun Zhu](https://ml.cs.tsinghua.edu.cn/~jun/index.shtml), [Lionel M. Ni](https://www.cse.ust.hk/~ni/), [Heung-Yeung Shum](https://scholar.google.com.hk/citations?user=9akH-n8AAAAJ&hl=en)

Code is under preparation, please be patient.

# News
[2022/6/7]: We release a unified detection and segmentation model [Mask DINO](https://arxiv.org/pdf/2206.02777.pdf) that achieves the best results on all the three segmentation tasks (**54.5** AP on [COCO instance leaderboard](https://paperswithcode.com/sota/instance-segmentation-on-coco-minival), **59.4** PQ on [COCO panoptic leaderboard](https://paperswithcode.com/sota/panoptic-segmentation-on-coco-minival), and **60.8** mIoU on [ADE20K semantic leaderboard](https://paperswithcode.com/sota/semantic-segmentation-on-ade20k))! Code will be available [here](https://github.com/IDEACVR/MaskDINO).
</br>
[2022/5/28] Code for [DN-DETR](https://arxiv.org/pdf/2203.01305.pdf) is available [here](https://github.com/IDEA-opensource/DN-DETR).
</br>
[2020/4/10]: Code for [DAB-DETR](https://arxiv.org/abs/2201.12329) is avaliable [here](https://github.com/SlongLiu/DAB-DETR).
</br>
[2022/3/8]: We reach the SOTA on [MS-COCO leader board](https://paperswithcode.com/sota/object-detection-on-coco) with **63.3AP**!
</br>
[2022/3/9]: We build a repo [Awesome Detection Transformer](https://github.com/IDEACVR/awesome-detection-transformer) to present papers about transformer for detection and segmenttion. Welcome to your attention!

# Abstract
We present **DINO** (**D**ETR with **I**mproved de**N**oising anch**O**r
boxes), a state-of-the-art end-to-end object detector. DINO improves
over previous DETR-like models in performance and efficiency by using
a contrastive way for denoising training, a mixed query selection method
for anchor initialization, and a look forward twice scheme for box prediction. DINO achieves **48.3**AP in 12 epochs and **51.0**AP in 36 epochs
on COCO with a ResNet-50 backbone and multi-scale features, yielding a significant improvement of +**4.9**AP and +**2.4**AP, respectively,
compared to DN-DETR, the previous best DETR-like model. DINO
scales well in both model size and data size. Without bells and whistles,
after pre-training on the Objects365 dataset with a SwinL backbone,
DINO obtains the best results on both COCO val2017 (**63.2**AP) and
test-dev (**63.3**AP). Compared to other models on the leaderboard,
DINO significantly reduces its model size and pre-training data size
while achieving better results.

# Results
![SOTA results](figs/sota.png "results on MSCOCO")
![sota table](figs/sota_table.png "optional title")
![12ep results](figs/12ep.png "optional title")
![50ep results](figs/50ep.png "optional title")
![curve table](figs/curve.png "optional title")

# Methods
![method](figs/model.png "model arch")

# Links
Our model is based on [DAB-DETR](https://arxiv.org/abs/2201.12329) and [DN-DETR](https://arxiv.org/abs/2203.01305).
<p>
<font size=3><b>DN-DETR: Accelerate DETR Training by Introducing Query DeNoising.</b></font>
<br>
<font size=2>Feng Li*, Hao Zhang*, Shilong Liu, Jian Guo, Lionel M. Ni, Lei Zhang.</font>
<br>
<font size=2>IEEE Conference on Computer Vision and Pattern Recognition (<b>CVPR</b>) 2022.</font>
<br>
<a href='https://arxiv.org/abs/2203.01305'>[paper]</a> <a href='https://github.com/FengLi-ust/DN-DETR'>[code]</a> <a href='https://www.zhihu.com/question/517340666/answer/2381304399'>[中文解读]</a>
</p>

<p>
<font size=3><b>DAB-DETR: Dynamic Anchor Boxes are Better Queries for DETR.</b></font>
<br>
<font size=2>Shilong Liu, Feng Li, Hao Zhang, Xiao Yang, Xianbiao Qi, Hang Su, Jun Zhu, Lei Zhang.</font>
<br>
<font size=2>International Conference on Learning Representations (<b>ICLR</b>) 2022.</font>
<br>
<a href='https://arxiv.org/abs/2201.12329'>[paper]</a> <a href='https://github.com/SlongLiu/DAB-DETR'>[code]</a>    
</p>


# Bibtex
If you find our work helpful for your research, please consider citing the following BibTeX entry.   
```
@misc{zhang2022dino,
      title={DINO: DETR with Improved DeNoising Anchor Boxes for End-to-End Object Detection}, 
      author={Hao Zhang and Feng Li and Shilong Liu and Lei Zhang and Hang Su and Jun Zhu and Lionel M. Ni and Heung-Yeung Shum},
      year={2022},
      eprint={2203.03605},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
