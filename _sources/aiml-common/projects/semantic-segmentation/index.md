# Semantic Segmentation of Satellite Imagery

![](satellites.jpeg)

You have been hired in the data science team at NASA and you are tasked to semantically segment objects that can be seen from space. 

**If you miss a milestone deadline you will be forfeited the corresponding points.**


## Milestone 1: Environment Preparation (10 points by 10/30)

You are given a seed repo for this project located [here](https://github.com/bnsreenu/python_for_microscopists) - look under the directory `228_semantic_segmentation_of_aerial_imagery_using_unet`.

1. Create a new repo under one Github account of a member of your team.
2. If you are working on own laptops/desktop: Checkout the code of the seed repo under src/ and incorporate [poetry](https://python-poetry.org/) to allow your virtual environment to set up properly. 
3. If you are working in Colab:  use pip to install all dependencies bearing in mind that Colab has built in TF/Pytorch installations. 
4. Install [NNI](https://nni.readthedocs.io/en/stable/index.html).  For Colab users: ensure that you have followed the instructions [here](https://nni.readthedocs.io/en/stable/sharings/nni_colab_support.html)  to allow the UI to be visible. 
5. Submit the github repository URL with a branch titled 'milestone-1' with the README.md file containing the installation instructions you followed and a screenshot of your computer of the NNI UI screen. Add as collaborator the TA.

## Milestone 2: Perform Baseline Semantic Segmentation (30 points by 11/6)

1. Watch this video that introduces [the dataset](https://www.kaggle.com/datasets/humansintheloop/semantic-segmentation-of-aerial-imagery) and the approach ([UNet](https://arxiv.org/abs/1505.04597)).
   
```{eval-rst}
.. youtube:: jvZm8REF2KY
```

2. Run the segmentation and produce plots of (a) 10 segmented images from the validation set (b) training and validation loss vs epochs, (b) Precision and Recall values  
3. Submit the github repository URL with a branch titled 'milestone-2' and with the docs/ folder containing the markdown file baseline-performance.md where you explain in 2 pages including figures UNet and in separate pages the results obtained. 

## Milestone 3 (CS301-101 ONLY): Hyperparameter Optimization (30 points by 11/20)

You are now tasked to improve baseline performance. 

1. Retrieve your team number from Canvas and consult the following table:

| Index | Method |
| --- | --- | 
| 1 | TPE |
| 2 | Anneal | 
| 3 | Evolution | 
| 4 | SMAC | 
| 5 | Hyperband | 
| 6 | Metis | 
| 7 | BOHB|
| 8 | GP | 
| 9 | DNGO | 

Team 1 is assigned method 1, ... Team 10 is assigned method 1, Team 11 is assigned method 2, etc.. Empty teams in canvas are also assigned their corresponding index - be careful to assign yourself the right method index and check with the adjacent team(s) to yours to be sure. 

2. Incorporate the Hyperparameter Optimization (HPO) method in your code and run the code to obtain the best (a) 10 segmented images from the validation set (b) training and validation loss vs epochs, (b) Precision and Recall values   

3. Submit the github repository URL with a branch titled 'milestone-3' and with the docs/ folder containing the markdown file hyperparameter-optimization.md where you explain in 2 pages including figures the method and in separate pages the results obtained. 

If you run out of compute resources i.e in Colab the GPU is taken away after few hours or your dedicated machine runs for ever or very slow, reduce the search space to produce results and achieve the milestone. If you reduce the space without any reason you will be deducted points. 

## Milestone 3 (CS301-103 ONLY): Neural Architecture Search (30 points by 11/20)

You are now tasked to do compress your model to fit a computer that may not have accelerator (GPUs) or enough memory to fit the original baseline model. Dont underestimate the impact of model compression - managing inference costs are the ranked consistently Number 1 goal for every enterprise that uses ML/AI.

1. Review the [seminal paper](https://arxiv.org/abs/1808.05377). 

2. Retrieve your team number from Canvas and consult the following table:

| Index | Method |
| --- | --- | 
| 1 | Random |
| 2 | GridSearch | 
| 3 | RegularizedEvolution | 
| 4 | TPE | 
| 5 | PolicyBasedRL | 
| 6 | DARTS | 
| 7 | ENAS|
| 8 | RandomOneShot | 
| 9 | ProxyLess | 

Team 1 is assigned method 1, ... Team 10 is assigned method 1, Team 11 is assigned method 2, etc.. Empty teams in canvas are also assigned their corresponding index - be careful to assign yourself the right method index and check with the adjacent team(s) to yours to be sure. 

1. Incorporate the NAS method in your code and run the code to obtain the best (a) 10 segmented images from the validation set (b) training and validation loss vs epochs, (b) Precision and Recall values   

2. Submit the github repository URL with a branch titled 'milestone-3' and with the docs/ folder containing the markdown file neural-arch-search.md where you explain in 2 pages including figures the method and in separate pages the results obtained. 

If you run out of compute resources i.e in Colab the GPU is taken away after few hours or your dedicated machine runs for ever or very slow, reduce the search space to produce results and achieve the milestone.

## Milestone 4: Model Compression (30 points by 12/04)

You are now tasked to do compress your model to fit a computer that may not have accelerator (GPUs) or enough memory to fit the original baseline model. Dont underestimate the impact of model compression - managing inference costs are the ranked consistently Number 1 goal for every enterprise that uses ML/AI.

1. Read about [the seminal paper](https://arxiv.org/abs/1503.02531)
2. Implement [Knowledge Distillation (KD)](https://nni.readthedocs.io/en/stable/sharings/kd_example.html) 
3. Run the code to obtain the student's network (a) 10 segmented images from the validation set (b) training and validation loss vs epochs, (b) Precision and Recall values 
4. Submit the github repository URL with a branch titled 'milestone-4' and with the docs/ folder containing the markdown file knowledge-distillation.md where you explain in 2 pages including figures the method and in separate pages the results obtained. 
