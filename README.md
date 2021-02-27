# Mental-Workload-Classification

Mental Workload is one of the major part of field of study known as ergonomics which is found to be influencing the productivity and performance of humans in a task. Hence it is important to assign tasks without overloading their mental state. This study is attempted to classify the mental workload on EOT crane operators who operate through computers and validate various predictors and the best model for the classification. Simulated tasks of different levels were designed and used for the experiment and various indicators were measured during the experiment. The 13 indicators that were measured in the experiment are eye’s fixation frequency, fixation duration on computer screen, saccade duration, saccade amplitude, fixation to saccade ratio, MD, PD, TD, P, E, FR, Score and RT (response time).The data is obtained from SAVR lab of Industrial Engineering Department, IIT Kharapur. During the experiment two types of mental workload (Hazard and Activity) are measured and labeled as positive (high mental workload imposed) and negative (low mental workload imposed). We propose an ensemble model of a neural network based model for the classification of mental workload. Two types of mental workloads can coexist. Hence our proposed base model is a multi-label classification model.

The Mental workload directory consists the entire files worked on during the project. Research papers contain the related Literature used for this study. 'reg.data114.csv' file consists dataset used for this project. The size of the dataset is 80 samples and each sample is a 13 dimensional feature vector. The 'datavisualization.py' contains code for visualizing the available data. The scatter plots for two labels and box plots for values of each feature are plotted. For scatter plots the 13 dimensional vector is transformed to 2-D using Principal Component Analysis. These plots are included in 'project_report.docx' in figures 2,3. The scripts 'Linear_Regression_Model.py' contains Linear Regression based ensemble model and 'single_hidden_layer.py', 'two_hidden_layers.py', 'three_hidden_layers.py' contains 1,2,3 layered neural network models along with ensemble learning implementation. The ensemble learning technique used in this study is bootstrap aggregation. The flow chart of this algorithm is shown in Figure 1 in project report. The results of the 4 models above are shown in Tables 1,2,3,4 in project report. The script 'plots.py' plots the variations of results obtained in terms of accuracy, hamming loss, precision, recall, f1-score and these plots can be seen in figures 4,5,6.

An improvement using Bootstrap Aggregation:
  The simple models of linear regression and neural networks gave an accuracy lying around 75%. After the use of this algorithm the accuracies were increased upto a range of 80-86%. These results are obtained by predicting on out of box examples for each model of ensemble. The limitation of this study is the lack of dataset(only 80 samples). Definitely there would be better results if more data is obtained.
