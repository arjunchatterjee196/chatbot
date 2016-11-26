## Retrieval-Based Conversational Model in Tensorflow (Ubuntu Dialog Corpus)

#### Overview

The code here implements the Dual LSTM Encoder model.

#### Setup

This code uses Python 3 and Tensorflow >= 0.9. Clone the repository and install all required packages:

```
pip install -U pip
pip install numpy scikit-learn pandas jupyter
```

#### Get the Data


Download the train/dev/test data [here](https://drive.google.com/open?id=0B_bZck-ksdkpVEtVc1R6Y01HMWM) and extract the acrhive into `./data`.


#### Training
§
```
python train.py
```


#### Evaluation

```
python test.py --model_dir=...

model_dir: 
    After executing the training script, depending on the time given to compute, the script will save the model data over time in the folder ./runs 
    Supply one of the created sub directories in runs as the parameter for model_dir to load that specific model

```


#### Evaluation

```
python predict.py --model_dir=...

model_dir: 
    After executing the training script, depending on the time given to compute, the script will save the model data over time in the folder ./runs 
    Supply one of the created sub directories in runs as the parameter for model_dir to load that specific model


```
