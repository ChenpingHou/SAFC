# SAFC
# # Code of SAFC(**Incremental Learning for Simultaneous Augmentation of Feature and Class**)

## Overview
This is the code for the paper "Incremental Learning for Simultaneous Augmentation of Feature and Class", which proposes a novel incremental learning method for Simultaneous
Augmentation of Feature and Class (SAFC). There are two main stages in the algorithm:
1. Data in stage 1 contains only C classes, and we first use data in stage 1 to build  a well learned model W1.
2. Data in stage 2 contains C+1 classes, and the dimension of data also increases. We reuse the model W1 learned in stage1 to train a new model on data in stage2.

## Main Files
There are two main files to implement SAFC method in the paper. 
 - SAFC_D.m: the method using direct constraint. There are five input parameters. 
                 - W1: The model learned in stage 1
 - train_data: the current training data. Each column represents an instance.
 - train_label: the label current training data. Each row represents an instance.
 - alpha and beta: two parameters in the paper.
 - SAFC_ID.m: the method using indirect constraint. There are five input parameters. 
                 - W1: The model learned in stage 1
 - train_data: the current training data. Each column represents an instance.
 - train_label: the label current training data. Each row represents an instance.
 - alpha and beta: two parameters in the paper.

 - demo.m: script that you can directly run on synthetic dataset. We use mysoftmax.m to build W1 in stage 1.

## Contact:
If there are any problems, please feel free to contact Chenping Hou (hcpnudt@hotmail.com).
