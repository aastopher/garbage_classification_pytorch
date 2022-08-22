# Garbage Classification with PyTorch
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwebstockreview.net%2Fimages%2Fgarbage-clipart-wastebin-16.png&f=1&nofb=1" alt="Garbage Bins" height="200"/>

---

## Goal

In this notebook we will implement different ResNet’s with the goal of comparing the models to find the 'best' for our classifier.

We are seeking to understand which ResNet configurations are most effective for classifying images of garbage. This type of modeling could be used for automated garbage aggregation systems.

## Model Comparison

<img src="res/MaxAcc.png" alt="MaxAcc" height="200"/> <img src="res/EvalAcc.png" alt="EvalAcc" height="200"/>

## Conclusion

Comparing ResNet models with an adam optimizer 8 epochs and a learning rate of 5.5e-5 for classification of garbage types yields a max model accuracy of 96% for the ResNet101 pretrained model. We should consider retraining the ResNet101 model with more epochs to locate where the accuracy fall off begins.

For reference, a good list of models and accuracies sit in pytorch’s docs: https://pytorch.org/vision/main/models.html