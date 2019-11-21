# DARTS: Differentiable Architecture Search

Hyojin Park, Lars Lowe Sjösund, YoungJoon Yoo, Nojun Kwak . "ExtremeC3Net: Extreme Lightweight Portrait Segmentation Networks using Advanced C3-modules" arXiv preprint [[arxiv](https://arxiv.org/abs/1908.03093)]

## Requirements

- python 3
- pytorch >= 0.4.0
- torchvision==0.2.1
- opencv-python==3.4.2.17
- numpy
- tensorboardX
- visdom

## Run example



- Train

```shell
python mainwithEdge.py
```
1) Stage1_ExtremeC3NetV2
    - stage1  train CoarseNet
    - stage2  train Full model
2) ExtremeC3Net_small
    - not use FineNet
    
- demo with video

```shell
# genotype from search results
python demo_video.py
```

## WeightFile

