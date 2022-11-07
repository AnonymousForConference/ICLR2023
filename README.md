# SAAL: Sharpness-Aware Active Learning

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Training

To train the model(s) in the paper, run this command:

```train
python main.py --data Cifar10 --acqMode Max_Diversity --optimizer_name Adam
```

## Evaluation

- Data will be downloaded to folder 'dataset'.
- Result will be recorded to folder 'Results'.

## Results

Our model achieves the following performance on active learning settings:

|  Optimizer   | FashionMNIST  |      SVHN     |    CIFAR-10   |   CIFAR-100   |
| ------------ |-------------- | ------------- | ------------- | ------------- |
|    Adam      |     85.8%     |     76.8%     |     54.4%     |     47.6%     |
|    SAM       |     86.3%     |     78.8%     |     57.0%     |     48.4%     |
