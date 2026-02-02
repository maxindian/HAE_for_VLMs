# Title: Hierarchical Adaptive Eviction for Vision-Language KV-Cache Efficiency
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
Code for the paper "**Hierarchical Adaptive Eviction for Vision-Language KV-Cache Efficiency**"
Authours: Xindian Ma, Yidi Lu, Peng Zhang, Jing Zhang. 
## Overview
The integration of visual information into Large Language Models (LLMs) has led to Multimodal Large Language Models (MLLMs), which enhance multimodal interactions. 
However, the increase in visual and text tokens results in high memory and computational costs due to the quadratic scaling of the Transformer architecture.
Due to the heterogeneous attention distribution between vision and language tokens, traditional eviction strategies treat all tokens uniformly and only consider 
the eviction of visual tokens, which either leads to performance degradation or suboptimal
memory optimization. 
In this paper, we propose a Hierarchical Adaptive Eviction (HAE) framework that prioritizes evicting visual tokens first, followed by joint recursive pruning of 
text and vision tokens based on dynamically reweighted attention scores. 
In the tasks of image understanding and long story generation evaluation, HAE reduces KV-Cache memory by 41%. In the image understanding task, the
average accuracy only dropped by 0.3%, and in the story generation experiments, it achieved a 1.5x inference speedup. Our work also formally demonstrates the
effectiveness of the HTV strategy in controlling set length and maintaining attribute similarity, 
providing a lightweight plug-in for real-time multimodal systems.

## Content
We provide two code to implement HEA for efficient multimodel understanding (image-based understanding) and generative inference (image-based StoryStream)
### HAE: Image-baed Understanding

### HAE: StoryStream
