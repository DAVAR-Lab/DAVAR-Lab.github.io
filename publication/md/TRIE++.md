# TRIE ++ : Towards End-to-End Information Extraction from Multiple Categories of Visually Rich Documents *(Under Review)*
### Abstract ##
Recently, automatically understanding visually rich documents (eg tickets and resumes) has become a hot and vital research topic due to its widespread commercial value. Most existing methods divide this task into two subparts: the text reading part for obtaining the plain text from the original document images and the information extraction part for extracting key contents. These methods mainly focus on improving the second, while neglecting that the two parts are highly correlated. This paper proposes a unified end-to-end document understanding framework, where text reading and information extraction can reinforce each other via a well-designed multi-modal context block. Specifically, the text reading part provides multi-modal features like visual, textual and layout features. The multi-modal context block is developed to fuse the generated multi-modal features and even the prior knowledge from the pre-trained language model for better semantic representation. The information extraction part is responsible for generating key contents with the fused context features. The framework can be trained in an end-to-end trainable manner, achieving global optimization. What is more, we define and group visually rich documents into four categories across two dimensions, the layout and text type. For each document category, we provide or recommend the corresponding benchmarks, evaluation protocols, experimental settings and strong baselines for remedying the problem that this research area lacks the uniform evaluation standard. Extensive experiments on four kinds of benchmarks (from fixed layout to variable layout, from full-structured text to semi-unstructured text) are reported, demonstrating the proposed method's effectiveness. Data, source code and models are available. We try our best to promote the research community, and data, code and models are available.

### Highlights Contributions
(1) We propose an end-to-end trainable framework for understanding visually rich documents, which can be trained end-to-end from scratch, with no need of stage-wise training strategies. 
(2) We implement the framework by simultaneously learning text reading and information extraction tasks via a well-designed multimodal context block, and also verify the mutual influence of text reading and information extraction. 
(3) To make evaluations more comprehensive and convincing, we define and divide VRDs into four categories. For each kind of documents, we provide the corresponding benchmarks, the evaluation protocols, experimental settings and even their strong baselines.
(4) Extensive evaluations on four kinds of real-world benchmarks show superior performance compared with the state-of-the-arts. Those benchmarks cover diverse types of document images, from fixed to variable layouts, from structured to semi-unstructured text types.

### More Results
For 'Strong Baselines on Four Categories of VRD', we also provide the entity-level evaluation results for Taxi invoice, Business email, Wildreceipt and Resume. See the [entity-results.xlsx](attachments/entity-results.xlsx) file.

### Evaluation Protocols
- For detection task, the precision (*abbr.*```PRE$_d$```), recall (*abbr.*```REC$_d$```) and F-measure (*abbr.*```F$_d$-m```) are calculated by following the [IoU evaluation strategy](https://rrc.cvc.uab.es/?ch=4&com=mymethods&task=1) in ICDAR 2015 robust reading competition. The IoU threshold is set to 0.5。
- For recognition task, the accuracy results (*abbr.*```ACC```) are shown as 
	<center><img src="attachments/acc.png" width="450"/></center>
   
    where a text is correctly predicted if and only if all characters are matched w.r.t its ground truth.
- For the end-to-end text spotting task, the precision (*abbr.*```PRE$_r$```), recall (*abbr.*```REC$_r$```) and F-measure (*abbr.*```F$_r$-m```) are same to the [end-to-end evaluation](https://rrc.cvc.uab.es/?ch=4&com=mymethods&task=1) in ICDAR 2015 robust reading competition.
- For the information extraction task, the entity precision (*abbr.*```ePRE```), entity recall (*abbr.*```eREC```) and entity F-measure (*abbr.*```eF1```) are used as
     <center><img src="attachments/ef1.png"width="450"/></center>
	
    where an extract text entity is treated as correct if its character content and category of the extracted text matches the groundtruth; Otherwise, denoted as incorrect. 
    

The evaluation scripts will be available in our code. 

### Codes and Models
Available at https://github.com/hikopensource/DAVAR-Lab-OCR (to be released)

### Datasets
Available at https://davar-lab.github.io/dataset/vrd.html

### Contact ##
If you have any questions about the dataset, please contact Zhanzhan Cheng (11821104@zju.edu.cn).

### Terms of Use ##
- The public annotations and trained models belong to the CSCG Group and are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).
- The images belong to Zhejiang University and are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

### Change Log ##
- 2021-10-08 (GMT+8): website create
