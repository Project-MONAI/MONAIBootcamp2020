# MONAIBootcamp2020

This repository hosts the notebooks for the 2020 MONAI Bootcamp event. The data required for the notebooks is available through the download mechanisms given in each notebook or through the organizers. All bootcamp participants can access the bootcamp Slack channel to ask for help with any issues. 


## Google Colab

The notebooks can be run in Google Colab by following these links. The Day 1 notebooks have the `pip` command for install MONAI, however this will have to be added to any subsequent notebook.
Place this at the top of the first cell to install MONAI the first time a colab notebook is run:

```
%pip install -qU "monai[nibabel,ignite,torchvision]==0.3.0rc2"
```

To use GPU resources through Colab remember to change the runtime to GPU:
1. From the "Runtime" menu select "Change Runtime Type"
2. Choose "GPU" from the drop-down menu
3. Click "SAVE"

This will reset the notebook and probably ask you if you are a robot (these instructions assume you are not). Running `!nvidia-smi` in a cell will verify this has worked and show you what kind of hardware you have access to. 

Google Drive files can be accessed by mounting your account in the notebook, this is a convenient way of accessing stored data. Add the following to a cell to mount your directory, you will be asked to authenticate through Google once you run it:

```python
from google.colab import drive

drive.mount('/content/drive')
!ls -l "/content/drive/My Drive/Colab Notebooks"
```

Day 1 Notebooks:
* [Lab 1 Transforms](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day1notebooks/lab1_transforms.ipynb)
* [Lab 2 End-to-End](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day1notebooks/lab2_end_to_end.ipynb)
* [Lab 3 Datasets](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day1notebooks/lab3_datasets.ipynb)
* [Lab 3 Networks](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day1notebooks/lab3_networks.ipynb)
* [Lab 3 Post Transforms](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day1notebooks/lab3_post_transforms.ipynb)

Day 2 Notebooks:
* [MedNIST GAN Tutorial](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day2notebooks/day2_mednist_GAN_tutorial.ipynb)
* [Cardiac Segmentation Challenge](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day2notebooks/day2_segment_challenge.ipynb) ([Solution](https://colab.research.google.com/github/Project-MONAI/MONAIBootcamp2020/blob/master/day2notebooks/day2_segment_challenge_solution.ipynb))
