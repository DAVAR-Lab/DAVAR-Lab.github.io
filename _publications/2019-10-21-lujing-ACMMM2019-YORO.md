---
title: "You Only Recognize Once: Towards Fast Video Text Spotting"
collection: publications
permalink: /publication/2019-10-21-lujing-ACMMM2019-YORO
excerpt: 'This paper is about video text spotting, pulished in ACMMM2019.'
date: 2019-10-21
venue: 'October 21'
citation: 'Zhanzhan Cheng, Jing Lu, Yi Niu et al. (2019). "You Only Recognize Once: Towards Fast Video Text Spotting." <i>October 21</i>. 1(1).' 
slides: '../files/2019-10-21-lujing-ACMMM2019-YORO-slides.pdf'
paperurl: '../files/2019-10-21-lujing-ACMMM2019-YORO-paper.pdf'
# code: '../files/%.zip'
# bibtex: ''              
---
Video text spotting is still an important research topic due to its various real-applications. 
Previous approaches usually fall into the four-staged pipeline: 
text detection in individual images, 
framewisely recognizing localized text regions, 
tracking text streams and 
generating final results with complicated post-processing skills, 
which might suffer from the huge computational cost as well as the interferences of low-quality text.
In this paper, we propose a fast and robust video text spotting framework by only recognizing the localized text one-time instead of frame-wisely recognition. 
Specifically, we first obtain text regions in videos with a well-designed spatial-temporal detector. 
Then we concentrate on developing a novel text recommender for selecting the highest-quality text from text streams and only recognizing the selected ones. 
Here, the recommender assembles text tracking, quality scoring and recognition into an end-to-end trainable module, 
which not only avoids the interferences from low-quality text but also dramatically speeds up the video text spotting process. 
In addition, we collect a larger scale video text dataset (LSVTD) for promoting the video text spotting community, 
which contains 100 text videos from 22 different real life scenarios. 
Extensive experiments on two public benchmarks show that our method greatly speeds up the recognition process averagely by 71 times compared with the frame-wise manner, 
and also achieves the remarkable state-of-the-art.
 
<br><br/>

<!-- BibTex here (Make sure that this is the last code block) -->
```
@article{123Xu2018Segregated,
  title={Segregated Temporal Assembly Recurrent Networks for Weakly Supervised Multiple Action Detection},
  author={Xu, Yunlu and Zhang, Chengwei and Cheng, Zhanzhan and Xie, Jianwen and Wu, Fei},
  year={2018},
}
```
