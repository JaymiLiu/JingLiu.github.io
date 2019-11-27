---
title: "Social media data analysis with Graph Neural Networks (GNN)"
---
## Predicting Influence Probabilities using Graph Convolutional Networks

### **Highlights**
+ Proposed a node-edge co-convolution graph neural network architecture
+ Demonstrated its effectiveness in predicting information diffusion (i.e., influence probability) over social networks  

The aim of this work is to predict the probability that one person influences another person over the social network so that it can more precisely to predicte information cascade over social network. Graph is used to model the social network, the influence probability to be predicted is one edge feature. We conjecture that the co-convolution of vertex features and edge features following the information flow direction could improve the prediction accuracy. The proposed node-edge co-convolution is illustrated as follows. The experiment result shows very high prediction accuracy with mean absolute percentage error less than 0.1.

Covolve Hidden vectors for node (left) and edge (right) following the information flow direction.

![GNN_1]({{ site.url }}{{ site.baseurl }}/assets/GCN_information_flow.png)

Overall Architecture

![GNN_2]({{ site.url }}{{ site.baseurl }}/assets/GCN_overall.png)


## VASE: A Twitter-based Vulnerability Analysis and Score Engine
### **Highlights**
- Proposed a novel attention-based input embedding layer which includes a bi-directional long short term memory (LSTM) network and an attention network to extract vulnerability-related information from tweet texts 
- Integrated the proposed input embedding layer with one state-of-the-art graph convolution neural network for predicting the severity of vulnerabilities

The aim of this work is to use Twitter discussions about vulnerabilities for predicting their severity before the assessments by official agencies. A GCN model is adopted in order to leverage the intrinsic correlations among vulnerabilities for prediction purpose. The graph is constructed in the following way. Each vulnerability is one node. To construct edge among vulnerabilities, tweet-contents related Features (i.e., Bag-of-Words, BoW) are first extracted for each vulnerability. One edge is drawn between two vulnerabilities if the cosine similarity of their BoW features is above a certain threshold. To further capture information contained in tweets, an attention-based input embedding layer is proposed and integrated with one state-of-the-art GCN network. This work could predict the severity of 37.85% volunerabilities at least one week earlier than the official agencies and with a mean absolute error or 1.255.

Attention-based input embedding layer

![CVSS_1]({{ site.url }}{{ site.baseurl }}/assets/attention_layer.png)

Overall Architecture

![CVSS_2]({{ site.url }}{{ site.baseurl }}/assets/CVSS_arct.png)


<!---
### Research Associate  
  Collaborator: Dr. Noseong Park
  George Mason University, Sep. 2018 to Aug. 2019
+ *Social media data analysis with Graph Neural Networks (GNN)*
  - Processed both unstructured (e.g., textual data) and structured (e.g., friendship relations and retweet records) social media data
  - Customized a bi-directional long short term memory (LSTM) network to embed tweet texts and integrated it with one state-of-the-art graph convolution neural network for predicting the severity of vulnerabilities, one cyber-security application, moving average to handle the out-of-memory issue for gpu, attention mechanism to get useful tweets
  - Proposed a node-edge co-convolution graph neural network architecture and demonstrated its effectiveness in predicting information diffusion (i.e., influence probability) over social networks  
+ *Data augmentation with Generative Adversarial Networks (GAN)*
	- Developed a GAN architecture to synthesize incomplete tabular data with two constraints that are maintaining column-wise statistical means and functional dependencies
	- Improved classification performance with synthesized data and outperformed various state-of-the-art data augmentation approaches
+ *Modeling and accelerating large-scale optimization problems with TensorFlow*
	- Proposed a neural network to model non-linear 0-1 knapsack problem and devised an adaptive gradient ascent method to solve the network 
	- Developed deep neural networks to model and maximize airline market share over air transportation network 
### Research Assistant
  Supervisor: Dr. Ming Lu
  University of Alberta, Sep. 2014 to Jul. 2018
+ Dual-Level Resource-Constrained Multi-Project Scheduling Framework for Prefabrication in Construction
  - Proposed a dual-level multi-project scheduling methodology to improve the resource allocation practice of multiple concurrent projects by enhancing the robustness of derived resource plans
  - Implemented the proposed methodology in *IBM ILOG CPLEX Optimization Studio* for proof-of-concept
  - Developed a MS project addon (in C#) for a partner construction company to apply the proposed methodology in scheduling bridge girder fabrication projects
### Research Assistant
  Supervisor: Dr. Fei Qiao
  Tsinghua University, Oct. 2010 to Jun. 2014
+ A novel low-complexity video compression method based on Underdetermined Blind Signal Separation (UBSS) and Compressive Sensing (CS)
+ Developed two video coding frameworks (in Matlab) which weigh recovery quality and decoding time, employed **TV** minimization by **A**ugmented **L**agrangian and **AL**ternating direction **AL**gorithms (TVAL3) as the decoding algorithm
+ Validated the effectiveness of the proposed method by comparing with two conventional video coding methods (i.e., H.264 and JPEG) and a well-known low-complexity video compression approach DISCOVER 
### Intern
  Advisor: Dr. Jiansong Zhang and [Dr. Kun Tan](http://kuntan.info/)
  Microsoft Research Asia (MSRA), Jun. 2011 to Aug. 2012 -->
