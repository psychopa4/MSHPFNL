# A Progressive Fusion Generative Adversarial Network for Realistic and Consistent Video Super-Resolution
This work is based on [Yi et al.](https://github.com/psychopa4/PFNL)
This is the TensorFlow version, and PyTorch version will be available.

## Datasets
We have selected [MM522 dataset](https://github.com/psychopa4/MMCNN) for training and collected another 20 sequences for evaluation, and in consider of copyright, the datasets should only be used for study.

The datasets can be downloaded from Google Drive and Baidu Drive, [train](https://drive.google.com/open?id=1xPMYiA0JwtUe9GKiUa4m31XvDPnX7Juu) and [eval,test,checkpoint](https://pan.baidu.com/s/1TNtkn_dHHQf_3_JABKWgZg) (password: pr7p).

Note that the [training](https://drive.google.com/open?id=1xPMYiA0JwtUe9GKiUa4m31XvDPnX7Juu) dataset provides Ground Truth images and Bicubic downsampling LR images, while the [eval](https://pan.baidu.com/s/1TNtkn_dHHQf_3_JABKWgZg) (password: pr7p) dataset provides Gaussian blur and downsampling images. Thus, please refer to ./model/base_model.py for generating Gaussian blur and downsampling images from Ground Truth images.

Unzip the training dataset to ./data/train/ and evaluation dataset to ./data/val/ .

## Environment
  - Python (Tested on 3.6)
  - Tensorflow (Tested on 1.12.0)

## Citation
If you find our code or datasets helpful, please consider citing our related works.
```
@ARTICLE{MSHPFNL,
  author={Yi, Peng and Wang, Zhongyuan and Jiang, Kui and Jiang, Junjun and Lu, Tao and Ma, Jiayi},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
  title={A Progressive Fusion Generative Adversarial Network for Realistic and Consistent Video Super-Resolution}, 
  year={2020},
  volume={},
  number={},
  pages={},
  doi={10.1109/TPAMI.2020.3042298}
}

@inproceedings{PFNL,
  title={Progressive Fusion Video Super-Resolution Network via Exploiting Non-Local Spatio-Temporal Correlations},
  author={Yi, Peng and Wang, Zhongyuan and Jiang, Kui and Jiang, Junjun and Ma, Jiayi},
  booktitle={IEEE International Conference on Computer Vision (ICCV)},
  pages={3106-3115},
  year={2019},
}
```

## Contact
If you have questions or suggestions, please open an issue here or send an email to yipeng@whu.edu.cn.