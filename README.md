# **HMNeRFBench: A Comprehensive Benchmark for Neural Human Radiance Fields**

![](./assets/logo.jpg)

<p align="center">
  <!-- <a href='https://arxiv.org/abs/2307.00818'>
    <img src='https://img.shields.io/badge/Arxiv-2307.00818-A42C25?style=flat&logo=arXiv&logoColor=A42C25'>
  </a> -->
  <a href='https://openreview.net/pdf?id=7kc4gtEk3b'>
    <img src='https://img.shields.io/badge/Paper-PDF-yellow?style=flat&logo=arXiv&logoColor=yellow'>
  </a>
  <a href='https://kenkunliu.github.io/HMNeRFBench/'>
  <img src='https://img.shields.io/badge/Project-Page-pink?style=flat&logo=Google%20chrome&logoColor=pink'></a>
  <!-- <a href='https://youtu.be/0a0ZYJgzdWE'>
  <img src='https://img.shields.io/badge/YouTube-Video-EA3323?style=flat&logo=youtube&logoColor=EA3323'></a> -->
  <a href='https://github.com/IDEA-Research/Motion-X'>
    <img src='https://img.shields.io/badge/GitHub-Code-black?style=flat&logo=github&logoColor=white'></a>
  <!-- <a href='LICENSE'>
    <img src='https://img.shields.io/badge/License-IDEA-blue.svg'>
  </a> -->
  <!-- <a href="" target='_blank'>
    <img src="https://visitor-badge.laobi.icu/badge?page_id=IDEA-Research.Motion-X&left_color=gray&right_color=orange">
  </a> -->
</p>

This repository contains the implementation of the following paper:
> A Comprehensive Benchmark for Neural Human Radiance Fields <br>[Kenkun Liu](https://kenkunliu.github.io/PersonalPage/)<sup>12</sup>, [Derong Jin](https://humathe.github.io/)<sup>2</sup>, [Ailing Zeng](https://ailingzeng.site)<sup>1</sup>, [Xiaoguang Han](https://gaplab.cuhk.edu.cn/pages/people)<sup>2</sup>, [Lei Zhang](https://www.leizhang.org/)<sup>1</sup><br>
> <sup>1</sup>International Digital Economy Academy  <sup>2</sup>The Chinese University of Hong Kong, Shenzhen

## Datasets ###
1. [ZJU-MoCap](https://github.com/zju3dv/neuralbody)
2. [GeneBody](https://github.com/generalizable-neural-performer/gnr)
3. [HuMMan](https://caizhongang.com/projects/HuMMan/recon.html)


## Unifying Settings
Comparisons of recent NeRF-based human rendering methods on different aspects. In the column Dataset, ZM, PS, GB, HM, H36M, RP are ZJU-MoCap, People-Snapshot, GeneBody, HuMMan, Human3.6M, RenderPeople datasets, respectively. Views: train views for scene-specific methods and input views (\*) for generalizable methods. Frames: train frames for scene-specific methods and input frames (\*) for generalizable methods

<div align="center">
<table cellspacing="0" cellpadding="0" bgcolor="#ffffff" border="0">
  <tr>
    <th align="center">Method</th>
    <th align="center">Dataset</th>
    <th align="center">Views</th>
    <th align="center">Frames</th>
    <th align="center">Generalizable</th>
    <th align="center">Animatable</th>
  </tr>
  <tr></tr>
  <tr>
    <td align="center"><b><a href="https://github.com/zju3dv/neuralbody">NeuralBody</a></b></td>
    <td align="center">ZM, PS</td>
    <td align="center">4</td>
    <td align="center">100-300</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/zju3dv/animatable_nerf">AniNeRF</a></b></td>
    <td align="center">ZM, H36M</td>
    <td align="center">4</td>
    <td align="center">100-300</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/taconite/arah-release">ARAH</a></b></td>
    <td align="center">ZM, H36M</td>
    <td align="center">4</td>
    <td align="center">300-400</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/chungyiweng/humannerf">HumanNeRF</a></b></td>
    <td align="center">ZM</td>
    <td align="center">1</td>
    <td align="center">500-600</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/fanegg/UV-Volumes">UV-Volume</a></b></td>
    <td align="center">ZM, H36M</td>
    <td align="center">18</td>
    <td align="center">100</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/Yzmblog/MonoHuman">MonoHuman</a></b></td>
    <td align="center">ZM</td>
    <td align="center">1</td>
    <td align="center">500-600</td>
    <td align="center">&#10008</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/YoungJoongUNC/Neural_Human_Performer">NHP</a></b></td>
    <td align="center">ZM, AIST++</td>
    <td align="center">3*</td>
    <td align="center">1* or 3*</td>
    <td align="center">&#10004</td>
    <td align="center">&#10008</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/gaoxiangjun/MPS-NeRF">MPS-NeRF</a></b></td>
    <td align="center">ZM, H36M, THuman</td>
    <td align="center">3*</td>
    <td align="center">1*</td>
    <td align="center">&#10004</td>
    <td align="center">&#10004</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/sail-sg/GP-Nerf">GP-NeRF</a></b></td>
    <td align="center">ZM</td>
    <td align="center">3*</td>
    <td align="center">1*</td>
    <td align="center">&#10004</td>
    <td align="center">&#10008</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/facebookresearch/KeypointNeRF">KeypointNeRF</a></b></td>
    <td align="center">ZM</td>
    <td align="center">3*</td>
    <td align="center">1*</td>
    <td align="center">&#10004</td>
    <td align="center">&#10008</td>
  </tr>
  <tr>
    <td align="center"><b><a href="https://github.com/generalizable-neural-performer/gnr">GNR</a></b></td>
    <td align="center">ZM, GB, RP</td>
    <td align="center">4*</td>
    <td align="center">1*</td>
    <td align="center">&#10004</td>
    <td align="center">&#10008</td>
  </tr>
</table>
</div>

## Benchmarking Scene-specific Methods (Coming soon...)

## Benchmarking Generalizable Methods (Coming soon...)

## [GeneHumanNeRF: Animatable and Generalizable Human NeRF from Monocular Videos](animation/GeneHumanNeRF/)

## 🤝 Citation  

If you find this repository useful for your work, please consider citing it as follows:

```  
@inproceedings{liu2023comprehensive,
        title={A Comprehensive Benchmark for Neural Human Radiance Fields},
        author={Liu, Kenkun and Jin, Derong and Zeng, Ailing and Han, Xiaoguang and Zhang, Lei},
        booktitle={Thirty-seventh Conference on Neural Information Processing Systems Datasets and Benchmarks Track},
        year={2023}
      }
```