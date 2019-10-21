---
title: "Segregated Temporal Assembly Recurrent Networks for Weakly Supervised Multiple Action Detection"
collection: publications
permalink: /publication/2018-11-11-xuyunlu-AAAI2019-STAR
excerpt: 'This paper is about video action detection task. We propose a segregated assembly recurrent called STAR network for weakly-supervised multiple action detection.'
date: 2018-11-11
venue: 'November 11'
citation: 'Yunlu Xu, Chengwei Zhang, Zhanzhan Cheng et al. (2018). "Segregated Temporal Assembly Recurrent Networks for Weakly Supervised Multiple Action Detection." <i>November 11</i>. 1(1).' 
slides: '../files/2018-11-11-xuyunlu-AAAI2019-STAR-slides.pdf'
paperurl: '../files/2018-11-11-xuyunlu-AAAI2019-STAR-paper.pdf'
# code: 'http://github.com/DAVAR-Lab/DAVAR-Lab.github.io'
bibtex: ''                                                                                                                                                                       
---
This paper proposes a segregated temporal assembly recurrent (STAR) network for weakly-supervised multiple action detection. 
The model learns from untrimmed videos with only supervision of video-level labels and makes prediction of intervals of multiple actions. 
Speciﬁcally, we ﬁrst assemble video clips according to class labels by an attention mechanism that learns class-variable attention weights and thus helps the noise relieving from background or other actions. 
Secondly, we build temporal relationship between actions by feeding the assembled features into an enhanced recurrent neural network. 
Finally, we transform the output of recurrent neural network into the corresponding action distribution. 
In order to generate more precise temporal proposals, we design a score term called segregated temporal gradient-weighted class activation mapping (ST-GradCAM) fused with attention weights. 
Experiments on THUMOS’14 and ActivityNet1.3 datasets show that our approach outperforms the state-of-the-art weakly-supervised method, and performs at par with the fully-supervised counterparts.



<br><br/>

<!-- BibTex here (Make sure that this is the last code block) -->
```
@article{123Xu2018Segregated,
  title={Segregated Temporal Assembly Recurrent Networks for Weakly Supervised Multiple Action Detection},
  author={Xu, Yunlu and Zhang, Chengwei and Cheng, Zhanzhan and Xie, Jianwen and Wu, Fei},
  year={2018},
}
```

