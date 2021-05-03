# Skin cancer detection

## Introduction

There were around 300,000 confirmed new cases of melanoma (malignant) skin cancer worldwide in 2018. During the same year, more than a million new non-melanoma (benign) cases were diagnosed. The numbers are most likely an underestimate due to various factors though (such as countries' lack of registries or wars). The Scandinavian counties are all ranked very high in terms of cancer rates per capita, where Sweden, my home country, is ranked 6th, averaged over both sexes.

A combination of very white skin and a society that considers being sun-tanned to be attractive likely contributes to these high numbers in Sweden. Being able to quickly and accurately check a spot on the skin can thus be desirable for many. By using deep learning techniques and a publicly available dataset, I will test the hypothesis on whether it's possible to classify melanoma skin cancer from non-melanoma skin cancer.

The dataset can be accessed on Kaggle through this [link](https://www.kaggle.com/fanconic/skin-cancer-malignant-vs-benign). There are in total 3,297 images, split into 2,110 train, 527 validation and 660 test images. It's a fairly small dataset, chosen specifically for computational bottlenecks. However, I will choose an implementation where the number of images can easily be scaled up to any number with practically no changes to the code.


## Summary and conclusions

If we are limited to current data, it might be better to go with the data augmented baseline as its performance is comparable to the larger Xception model but is faster to train, takes less space on disk and is in general less complex. It's also more reliable than the baseline without augmented data. However, if there is a way to collect more data, the Xception model will likely do significantly better across most, if not all, metrics.

We can conclude that it is possible to classify malignant from benign skin cancer using deep learning. Future work should start by collecting more data as it will likely yield the largest improvements.



