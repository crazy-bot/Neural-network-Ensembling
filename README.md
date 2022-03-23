# Neural Network Ensemble

This project is to demonstrate training and evaluation of ensembling of neural network base learners using soft voting aggregation. Everything is compiled in the [main.ipynb](ipython notebook)


# Network architecture:
The network configurations are provided in [model_configs.yaml](model_configs.yaml) and configurable with different no of layers, number of hidden units and learning rate.
I have used 5 Fully connected NN with simpler to more complex architecture and different learning rate. Training is done using stratified 5-fold cross validation. Each base learner is trained on 4 different subsets and validated on hold out subset.

# Dataset
Tabular data is used for this project. Data is kept inside [data] as csv files. Ths is multi class classification task with 10 different classes.
- train data : 24000 rows and 393 colums
- valid data : 6000 rows and 393 colums
- test data : 10000 rows and 393 columns


# evaluation results
I have saved training and validation loss and accuracy metric plots 
<p float="left">
  <img src="graphs/train_acc_model_0.svg" width="100" />
  <img src="graphs/train_acc_model_1.svg" width="100" /> 
  <img src="graphs/train_acc_model_2.svg" width="100" />
</p>

![](images/fakes.png)
![](images/fakes_mask.png)

# Future Scope
I have tried simple ensembling technique for the demonstration. We can use more advanced ensembling, sampling, subset feature selection, stacking based models as well.









