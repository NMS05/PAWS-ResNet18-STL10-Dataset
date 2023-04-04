# PAWS-ResNet18-STL10-Dataset


Colab Notebook providing a simple PyTorch implementation of [PAWS (Predicting View Assignments with Support samples)](https://openaccess.thecvf.com/content/ICCV2021/papers/Assran_Semi-Supervised_Learning_of_Visual_Features_by_Non-Parametrically_Predicting_View_Assignments_ICCV_2021_paper.pdf) using a ResNet18 model and [STL-10 dataset](https://cs.stanford.edu/~acoates/stl10/). The model can be trained on Google Colab with a single GPU.

**PAWS_train.py** - Train ResNet18 model with PAWS objective on the 100k unlabeled images of STL10 dataset for 50 epochs

**PAWS_eval.py** - Evaluate the quality of the pretrained representations with linear probing (trainable linear classifier with frozen backbone) on the labeled images of STL10 dataset.



### Performance (Accuracy)

  - **Random Weights** - 23.65%
  
  - **PAWS Weights** - 58.29%



### Code References
  1. [PAWS](https://github.com/facebookresearch/suncet)
  2. [AI Summer](https://github.com/The-AI-Summer/simclr)
