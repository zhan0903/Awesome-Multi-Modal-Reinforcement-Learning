# MMRL
# Awesome Multi-Modal Reinforcement Learning 

This is a collection of research papers for **Multi-Modal reinforcement learning (MMRL)**.
And the repository will be continuously updated to track the frontier of MMRL. 
Some papers may not be relevant to RL, but we include them anyway as they may be useful for the research of MMRL.

Welcome to follow and star!

<!-- <pre name="code" class="html">
<font color="red">[2022.07.06] New: We update the ICML 2022 paper list of model-based rl!

[2022.02.13] We update the ICLR 2022 paper list of model-based rl.</font>
</pre> -->


<!-- ## Table of Contents

- [A Taxonomy of RL](#a-taxonomy-of-model-based-rl-algorithms)
- [Papers](#papers)
  <!-- - [MARL](#classic-model-based-rl-papers)
  - [Offline RL](#icml-2022) 
  - [Meta RL](#iclr-2022) 
  - [OfflineToOnline RL](#neurips-2021)
  - [VisionBased RL](#iclr-2021)
  - [LanguageBased RL](#icml-2021) -->
<!-- - [Contributing](#contributing) -->


## A Introduction of Multi-Modal RL Algorithms

<!-- We’ll start this section with a disclaimer: it’s really quite hard to draw an accurate, all-encompassing taxonomy of algorithms in the Multi-Modal RL space, because the modularity of algorithms is not well-represented by a tree structure. So we will publish a series of related blogs to explain more Model-Based RL algorithms. -->

Multi-Modal RL agents focus on learning from video (images), language (text), or both, as humans do. We believe that it is important for intelligent agents to learn directly from images or text, since such data can be easily obtained from the Internet.

<!-- <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="./assets/mbrl-taxonomy.png">
    <br>
    <center>A non-exhaustive, but useful taxonomy of algorithms in modern Model-Based RL.</center>
</center> -->

<!-- We simply divide `Model-Based RL`  into two categories: `Learn the Model` and `Given the Model`. 
- `Learn the Model` mainly focuses on how to build the environment model. 
- `Given the Model` cares about how to utilize the learned model. 

And we give some examples as shown in the figure above. There are links to algorithms in taxonomy. -->

<!-- >[1] [World Models](https://worldmodels.github.io/): Ha and Schmidhuber, 2018  
[2] [I2A](https://arxiv.org/abs/1707.06203) (Imagination-Augmented Agents): Weber et al, 2017  
[3] [MBMF](https://sites.google.com/view/mbmf) (Model-Based RL with Model-Free Fine-Tuning): Nagabandi et al, 2017  
[4] [MBVE](https://arxiv.org/abs/1803.00101) (Model-Based Value Expansion): Feinberg et al, 2018  
[5] [ExIt](https://arxiv.org/abs/1705.08439) (Expert Iteration): Anthony et al, 2017  
[6] [AlphaZero](https://arxiv.org/abs/1712.01815): Silver et al, 2017  
[7] [POPLIN](https://openreview.net/forum?id=H1exf64KwH) (Model-Based Policy Planning): Wang et al, 2019  
[8] [M2AC](https://arxiv.org/abs/2010.04893) (Masked Model-based Actor-Critic): Pan et al, 2020
 -->


## Papers

```
format:
- [title](paper link) [links]
  - authors.
  - key words.
  - experiment environment.
```

- [MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge](https://arxiv.org/abs/2206.08853)
  - Linxi Fan, Guanzhi Wang, Yunfan Jiang, etc.
  - Key Words: multimodal dataset, MineClip
  - ExpEnv: Minecraft


- [SOAT: A Scene-and Object-Aware Transformer for Vision-and-Language Navigation](https://arxiv.org/pdf/2110.14143.pdf)
  - Abhinav Moudgil, Arjun Majumdar,Harsh Agrawal,etc, NeurIPS2021.
  - Key Words: Vision-and-Language Navigation
  - ExpEnv: Room-to-Room, Room-Across-Room

- [Recurrent World Models Facilitate Policy Evolution](https://papers.nips.cc/paper/2018/hash/2de5d16682c3c35007e4e92982f1a2ba-Abstract.html)
  - David Ha, Jürgen Schmidhuber, NeurIPS2018.
  - Key Words: World model,generative RNN,VAE
  - ExpEnv: VizDoom, CarRacing

- [Mastering Atari with Discrete World Models](https://arxiv.org/abs/2010.02193)
  - Danijar Hafner, Timothy Lillicrap, Mohammad Norouzi, etc. *ICLR2021*
  - Key Words: World models
  - ExpEnv: Atari

- [Offline Reinforcement Learning from Images with Latent Space Models](https://proceedings.mlr.press/v144/rafailov21a.html)
  - Rafael Rafailov, Tianhe Yu, Aravind Rajeswaran, etc. *ICML2021*
  - Key Words: Latent Space Models
  - ExpEnv: DeepMind Control,Adroit Pen,Sawyer Door Open,D’Claw Screw

- [Pretraining Representations for Data-Efﬁcient Reinforcement Learning](https://papers.nips.cc/paper/2021/hash/69eba34671b3ef1ef38ee85caae6b2a1-Abstract.html)
  - Max Schwarzer, Nitarshan Rajkumar, Michael Noukhovitch,etc. *NeurIPS2021*
  - Key Words: latent dynamics modelling,unsupervised RL
  - ExpEnv: Atari

- [LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action](https://arxiv.org/abs/2207.04429)
  - Dhruv Shah, Blazej Osinski, Brian Ichter,etc.
  - Key Words: CLIP,ViNG,GPT-3
  - ExpEnv: None

- [Learning Generalizable Robotic Reward Functions from “In-The-Wild” Human Videos](https://arxiv.org/abs/2103.16817)
  - Annie S. Chen, Suraj Nair, Chelsea Finn. *RSS2021*
  - Key Words: Reward Functions,“In-The-Wild” Human Videos
  - ExpEnv: None

- [Reinforcement Learning with Videos: Combining Ofﬂine Observations with Interaction](https://arxiv.org/abs/2011.06507)
  - Karl Schmeckpeper, Oleh Rybkin, Kostas Daniilidis,etc. *CoRL2020*
  - Key Words: learning from videos
  - ExpEnv: robotic pushing task, Meta-World

- [Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents](https://arxiv.org/pdf/2201.07207.pdf)
  - Wenlong Huang, Pieter Abbeel, Deepak Pathak,etc.
  - Key Words: large language models,Embodied Agents
  - ExpEnv: VirtualHome

- [Reinforcement Learning with Action-Free Pre-Training from Videos](https://proceedings.mlr.press/v162/seo22a.html)
  - Younggyo Seo, Kimin Lee, Stephen L James,etc. *ICML2022*
  - Key Words: action-free pretraining,videos
  - ExpEnv: Meta-world, DeepMind Control Suite

- [History Compression via Language Models in Reinforcement Learning](https://arxiv.org/abs/2205.12258)
  - Fabian Paischer, Thomas Adler, Vihang Patil,etc. *ICML2022*
  - Key Words: Pretrained Language Transformer
  - ExpEnv: Minigrid,Procgen

- [Learning Actionable Representations with Goal-Conditioned Policies](https://arxiv.org/abs/1811.07819)
  - Dibya Ghosh, Abhishek Gupta, Sergey Levine. *ICLR2019*
  - Key Words: Actionable Representations Learning
  - ExpEnv: 2D navigation

- [Is Cross-Attention Preferable to Self-Attention for Multi-Modal Emotion Recognition?](https://arxiv.org/abs/2202.09263)
  - Vandana Rajan, Alessio Brutti, Andrea Cavallaro. *ICASSP2022*
  - Key Words: Multi-Modal Emotion Recognition,Cross-Attention
  - ExpEnv: None.

- [How Much Can CLIP Benefit Vision-and-Language Tasks?](https://openreview.net/forum?id=zf_Ll3HZWgy)
  - Sheng Shen, Liunian Harold Li, Hao Tan,etc. *ICLR2022*
  - Key Words: Vision-and-Language,CLIP
  - ExpEnv: None.

- [Grounding Language to Entities and Dynamics for Generalization in Reinforcement Learning](https://arxiv.org/abs/2101.07393)
  - Austin W. Hanjie, Victor Zhong, Karthik Narasimhan. *ICML2021*
  - Key Words: Multi-modal Attention
  - ExpEnv: Messenger


- [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551)
  - Danijar Hafner, Timothy Lillicrap, Ian Fischer, etc. *ICML2019*
  - Key Words: latent dynamics model,pixel observations
  - ExpEnv: DeepMind Control Suite

- [Decoupling Representation Learning from Reinforcement Learning](https://arxiv.org/abs/2009.08319)
  - Adam Stooke,Kimin Lee,Pieter Abbeel, etc. *ICML2021*
  - Key Words: representation learning, unsupervised learning
  - ExpEnv: DMControl, Atari,DMLab

- [Masked Visual Pre-training for Motor Control](https://arxiv.org/abs/2203.06173)
  - Tete Xiao,Ilija Radosavovic,Trevor Darrell, etc. 
  - Key Words: self-supervised learning,motor control
  - ExpEnv: PixMC


## Contributing
Our purpose is to make this repo even better. If you are interested in contributing, please refer to [HERE](CONTRIBUTING.md) for instructions in contribution.


## License
Awesome Multi-Modal Reinforcement Learning is released under the Apache 2.0 license.
