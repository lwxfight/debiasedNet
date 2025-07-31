# DTSF-Net
[PR 2025] From Temporal Thumbnail to Semantics: Debiasing Multi-View Action Recognition
[[paper](https:)]   
![figure](/framework.png)
# From Temporal Thumbnail to Semantics: Debiasing Multi-View Action Recognition
<!-- ## News🚀
* **2024.09.27**: Our code is released.
* **2024.09.26**: Our inference code has been updated, and the code for selecting exemplars and the training code will be coming soon.
* **2024.07.02**: VA-Count is accepted by ECCV2024. -->
## Abstract 
Multi-view action recognition has garnered significant attention due to the challenges of view variation and dynamic feature modeling. Through comprehensive analysis, we uncover two previously overlooked biases, static bias within each view and view bias arising from asymmetric information distribution, that significantly undermine the generalization and robustness of feature representations, particularly under occlusion and complex motion. Motivated by these findings, we introduce the Debiased Temporal-Semantic Fusion Network (DTSFNet), which integrates a Temporal Snapshots Module to explicitly separate static and dynamic information via downsampled frame embeddings and leverages a Mamba-based semantic uncertainty fusion mechanism to dynamically weight each view during feature integration. DTSFNet achieves state-of-the-art accuracy (97.0% on N-UCLA and 96.7% on NTU-RGB+D) while maintaining high efficiency, requiring only 1.35 h of training, 725.08 GFLOPs, and 25.4 M parameters on N-UCLA. Extensive ablation studies and visualizations on N-UCLA and CASIA further validate the effectiveness and interpretability of our approach.

## Environment
```
pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu118
pip install -r requirements.txt
pip install -e causal-conv1d
pip install -e mamba
```
<!-- ### For more information on Grounding DINO, please refer to the following link: 
[GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
We are very grateful for the Grounding DINO approach, which has been instrumental in our work！ -->

## Datasets

* [NTU-RGB+D](https://rose1.ntu.edu.sg/dataset/actionRecognition/)

* [N-UCLA](https://wangjiangb.github.io/my_data.html)

* [CASIA](http://www.cbsr.ia.ac.cn/english/Action%20Databases%20EN.asp)



## Citation

```
@inproceedings{DTSF2025,
  title={From Temporal Thumbnail to Semantics: Debiasing Multi-View Action},
  author={Wei Feng, Zixian Zhu, Wenxuan Liu, Xu Wang, Bingyi Liu, Xiaohan Yu, Xian Zhong},
  booktitle={Proc. {IEEE/CVF} Conf. Comput. Vis. Pattern Recognit.},
  year={2025}
}
```

## Acknowledgement
This work was partly supported by the National Natural Science Foundation of China under Grant 62271361, the Hubei Provincial Key Research and Development Program under Grant 2024BAB039, and the Hubei Key Laboratory of Inland Shipping Technology under NHHY2024003. The authors acknowledge Beijing PARATERA Technology Co., LTD for providing high-performance and AI computing resources. 


#### If you have any questions, please get in touch with me (zhongx@whut.edu.cn).
