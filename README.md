<h1 align="center">
  <br>
  Vision Transformers for Galaxy Morphology Classification: <br> Fine-Tuning Pre-Trained Networks vs. Training From Scratch
  <br>
  <br>
  <img src="https://www.esa.int/var/esa/storage/images/esa_multimedia/videos/2013/11/guide_to_our_galaxy/13409760-3-eng-GB/Guide_to_our_Galaxy_pillars.png" alt="Markdownify" width="400">
</h1>

<h4 align="left">Abstract: </h4>  
<p class="tab">In recent years, the Transformer-based deep learning architecture has become extremely popular for downstream tasks, especially within the field of Computer Vision. However, transformer models are very data-hungry, making them challenging to adopt in many applications where data is scarce. Using transfer learning techniques, we explore the classic Vision Transformer (ViT) and its ability to transfer features from the natural image domain to classify images in the galactic image domain. Using the weights of models trained on ImageNet (a popular benchmark dataset for Computer Vision), we compare the results of two distinct ViTs: one base ViT (without pre-training) and another fine-tuned ViT pre-trained on ImageNet. Our experiments on the Galaxy10 dataset show that by using the pre-trained ViT model, we can get better accuracy compared to the ViT model built from scratch and do so with a faster training time. Experimental data further shows that the fine-tuned ViT model can achieve similar accuracy to the model built from scratch while using less training data.</p>


<br>
  <i><b>Vision Transformers for Galaxy Morphology Classification: Fine-Tuning Pre-Trained Networks vs. Training From Scratch</i></b> was written by <b>Rahul Kumar</b> under the supervision of <b>Dr. Mohammed Kamruzzaman Sarker</b> (advisor) and  <b>Dr. Sheikh Rabiul Islam</b> (coadvisor). This thesis has been submitted to the honors committee at the <b>University of Hartford</b>.


## PDF version
A rendered PDF version of the thesis can be found in the [research_publication_vit.pdf](/research_publication_vit.pdf) file. This paper was submitted to the DeLTA conference which is being held in Rome, Italy for 2023.

## Requirements
Once you have downloaded the project, locate the [requirements.txt](/requirements.txt) file using your terminal. From there, run
``` bash
pip install -r requirements.txt
```
and all of the required libraries will be downloaded. 

## Getting Started
There are two folders within this project: data and models. For the purposes of these experiments, we use Jupyter Notebook to conduct and monitor each of the experiements using the Vision Transformer (ViT). Once you have downloaded all the requirements, go into the [data.ipynb](/data/data.ipynb) file and change the paths where you want the data to be saved. Then, run the whole script to ensure that you have downloaded the galactic images. 
<br><br>
Next, you can examine the model performances at each dataset size as well as models with no weights and pre-trained weights. To access the ViT with no pre-trained weights, the file is named [visiontransformer-scratch.ipynb](/models/visiontransformer-scratch.ipynb). Otherwise, the other models all utilized pre-trained weights from the ViT trained on the ImageNet-1k dataset. The number at the end of each file represents the percentage of the dataset used to train the model (e.g [[visiontransformer_90.ipynb](/models/visiontransformer_90.ipynb)] = 90% of original dataset size, etc.)
<br><br>
Finally, the [plot.ipynb](/models/plot.ipynb) file contains the graphs and charts used for the publication draft. 

## Authors

Contributor names and contact info:

Rahul Kumar
* Email: kumarrah2002@gmail.com
* [LinkedIn](https://www.linkedin.com/in/kumarrah/)
* [GitHub](https://github.com/kumarrah2002)

Dr. Md Kamruzzaman Sarker
* Email: sarker@hartford.edu
* [GitHub](https://github.com/md-k-sarker)

Dr. Sheikh Rabiul Islam
* Email: shislam@hartford.edu
* [GitHub](https://github.com/SheikhRabiul)


## Acknowledgements

This research was conducted with the support of the University of Hartford
through the Vincent Coffin Grant (ID:398131).

## License
This thesis is made available under the GNU General Public License v3.0. A copy of the full license is available in the [LICENSE](/LICENSE) file.
