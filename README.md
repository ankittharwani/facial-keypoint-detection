# Facial Keypoint Detection

**Explorations on facial image keypoint detection.**  

This project contains the explorations on face feature detection (for the [Kaggle competition](https://www.kaggle.com/c/facial-keypoints-detection)), as part of the final project for the 207-Machine Learning course for [Berkeley's Master in Information and Data Science](https://datascience.berkeley.edu/).  

The project was developed by: [Alex](https://github.com/keivahn), [Ankit](https://github.com/ankittharwani), [Nina](https://github.com/kuknina) and [Will](https://github.com/willahscott).  


## Presentation
We created a [Prezi adventure](https://prezi.com/an_apyqfaeaj/recognizing-key-facial-points/#) to showcase our ideas and explorations.


## Final Notebook  

The notebook [FacialKeypointDetection-AlexAnkitNinaGuillermo](https://github.com/WillahScott/facial-keypoint-detection/blob/master/scripts/final-notebook/FacialKeypointDetection-AlexAnkitNinaGuillermo.ipynb) located in `scripts/final-notebook/` contains the final report summarizing most of the work included in the rest of the repository.  

For a full exposition refer to this notebook. However, this notebook is better treated as a report, than a runnable notebook, due to its size and its lengthy write-ups. For details on the runned codes refer to the specific notebooks, as guided by the READMEs.  


## Contents  

* **`scripts/`**  

	* **`explorations/`** contains dataset explorations, plots and initial modeling attempts  

    * **`preprocessors/`** contains the preprocessing scripts  

	* **`modelers/`** contains all serious modeling attempts, including the generation of their submission files

	* **`tools/`** contains a set of additional tools that make the exploration and modeling cleaner. For example `submit.py` contains functions for creating the submission files in the appropriate folder  

* **`data/`**  

	* **`datasets/`** contains the original kaggle data  

	* **`submissions/`** contains the csv files submitted to the Kaggle competition  

	* **`models/`** contains the persistent storages of the models created. Each pickled model contains: name, alias, description, model-object, prediction-df, [training-time], [predicting-time]  

	* **`preprocessed/`** contains preprocessed datasets. For *temporal* time-consuming preprocessings   
  

## Pre-requisites

* First of all clone the repo's folder:

```bash
$ git clone https://github.com/WillahScott/facial-keypoint-detection.git
```

Use of a **virtual environment** is highly recommended (specially through [*conda*](http://conda.pydata.org/docs/using/envs.html)).  

*Should you choose to not create a virtualenv and just install directly on your raw machine just install the prereqs (follow step 2 for virtualenv instructions)*  


### With `conda`

*  Clone the environment as provided in `environment.yml`:  
```bash
$ conda env create -f environment.yml
$ source activate fkd
```
That's it!  
*For more info on using virtual environments with conda see [here](http://conda.pydata.org/docs/using/envs.html)*

### With `virtualenv`  

* Create a virtual env (from within the folder) and activate it:  
```bash
$ cd facial-keypoint-detection
$ virtualenv fkd
$ source fkd/bin/activate
```  
* Install pre-reqs:
```bash
$ pip install -r requirements.txt
```
  

## Usage  

Refer to the subfolders README's for more details on the sections, contents and usage.  

*Last update: April, 2016*
