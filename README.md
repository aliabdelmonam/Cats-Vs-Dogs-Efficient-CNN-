# Cat vs Dog Image Classification


### Overview

The goal of this project is to classify images of cats and dogs. This is a common benchmark task in computer vision. By using **`EfficientNetV2M`** as the base model and fine-tuning it with additional dense layers, the model achieved high accuracy on the task.

## Model Architecture

- **Base Model**: `EfficientNetV2M` (pretrained on ImageNet)
- **Additional Layers**: `Global Average Pooling` and `Dense` layers added to enhance feature extraction
- **Output**: Softmax layer with 2 units (for cat and dog classes)


## Training Process

- **Dataset**: [Dogs vs Cats](https://www.kaggle.com/datasets/salader/dogs-vs-cats)
- **Data Augmentation**: Performed to improve model generalization.
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Evaluation Metric**: Accuracy
- **Model Checkpointing**: Saved the model with the best validation accuracy during training.

## Results

- **Final Accuracy**: 99.5%
