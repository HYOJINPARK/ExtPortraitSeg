# Extreme Lightwegith Portrait Segmentation


We apologize to close this GitHub due to some issue.
Our code will be released in this [link](https://github.com/clovaai) after security check.
I guess next week.
However if you have questions, please mail to me.
I am happy to wait for your question mail.
wolfrun@snu.ac.kr

## Requirements

- python 3
- pytorch >= 0.4.1
- torchvision==0.2.1
- opencv-python==3.4.2.17
- numpy
- tensorboardX
- visdom

## Model
ExtremeC3Net ([paper](https://arxiv.org/abs/1908.03093))

Hyojin Park, Lars Lowe Sjösund, YoungJoon Yoo, Nojun Kwak.
 
"ExtremeC3Net: Extreme Lightweight Portrait Segmentation Networks using Advanced C3-modules"

- config file : extremeC3Net.json
- Param : 0.038 M
- Flop : 0.128 G
- IoU : 94.98

SINet (will be soon)

Hyojin Park, Lars Lowe Sjösund, YoungJoon Yoo, Nicolas Monet, Nojun Kwak

SINet: Extreme Lightweight Portrait Segmentation Networks with Spatial Squeeze Modules and Information Blocking Decoder

- config file : SINet.json
- Param : 0.087 M
- Flop : 0.064 G
- IoU : 95.29 
## Run example



- Train

Download datasets 


1 . ExtremeC3Net
   
```shell
python main.py --c ExtremeC3Net.json
```
2 . SINet (soon)
   
```shell
python main.py --c SINet.json
```
 
 
## Trained model

will be soon

## Additonal Dataset

We make augmented dataset from Baidu fashion dataset.

The original Baidu dataset link is [here](http://www.cbsr.ia.ac.cn/users/ynyu/dataset/)

EG1800 dataset link what I used in [here](https://drive.google.com/file/d/1QmMrv7h-NJHYMnFfsqzqAM8d-G1Tz7VV/view?usp=sharing) 

Our augmented dataset will be open again. 
We use all train and val dataset for training segmentation model. 

## Citation
If our works is useful to you, please add two papers.
```shell
@article{park2019extremec3net,
  title={ExtremeC3Net: Extreme Lightweight Portrait Segmentation Networks using Advanced C3-modules},
  author={Park, Hyojin and Sj{\"o}sund, Lars Lowe and Yoo, YoungJoon and Kwak, Nojun},
  journal={arXiv preprint arXiv:1908.03093},
  year={2019}
}

SINet: Extreme Lightweight Portrait Segmentation Networks with Spatial Squeeze Modules and Information Blocking Decoder
( Soon )

```

## Acknowledge
We are grateful to [Clova AI, NAVER](https://github.com/clovaai) with valuable discussions.

I also appreciate my co-authors Lars Lowe Sjösund and YoungJoon Yoo from  [Clova AI, NAVER](https://clova.ai/en/research/research-areas.html),
and  Nicolas Monet from [NAVER LABS Europe](https://europe.naverlabs.com/).
