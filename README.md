Code for the paper Local Label Propagation with Class Attention for Effective and Efficient Hyperspectral Images Classification submitted to IEEE GRSL


# LLPCA
- Local Label Propagation (LLP).
- Local Label Propagation with Class Attention (LLPCA).

## Parameter:
The data sets and  number of training samples can be selected within the code.  
- DataSetName in {'Indianpines', 'PaviaU', 'HongHu'}
- number indicates the number of training samples selected for each category.
- d indicates the radius.
- k indicates the minimum threshold for the number of allowed propagations in CA mask.(only for LLPCA)

## Usage:
For example, when DataSet Indianpines takes 5-30 training sample points for each class, the method of calling LLP and LLPCA algorithm for "Indianpines" is as follows:
- LLP("Indianpines",[5,10,15,20,25,30],2);
- LLPCA("Indianpines",[5,10,15,20,25,30],1,10);


## Images:
The following figure illustrates the process of the proposed LLPCA.

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/LLPCA_progress.png?raw=true)


The following figure illustrates the label propagation in different scenarios of the proposed LLP, corresponding to: (1) no labeled samples in the local area, (2) labeled samples present in the local area, and (3) no labeled samples in the local area, but labeled samples present within the local areas of neighboring samples.

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/LLP.png?raw=true)


The following figure presents the flowchart of the proposed Class Attention, with an example shown for K=4.

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/CA.png?raw=true)


The following figure presents the classification maps from the proposed LLPCA on the three HSIs data.

Indian Pines:

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/indian.png?raw=true)


PaviaU:

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/paviau.png?raw=true)


HongHu:

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/honghu.png?raw=true)


## Tables:
The following table presents the experimental results of LLPCA on imbalanced samples, using the Indian Pines dataset as an example.

![Alt text](https://github.com/nmvbxcz/LLPCA/blob/main/imbalanced_samples.png?raw=true)
