# Yandex Cup 2023 (RecSys)
Automatic music genre classification is one of applied tasks of Yandex Music service. Millions of music tracks are available on this service now and manual labeling of tracks is not efficient. The goal of this contest is development of ML model predicts music genre from it's embeddings. Average Precision (AP) metric is used for model quality measurement.
In this project **Pytorch** framework is used for model training and inference. **Torchmetrics**, **Pandas**, **Numpy** and **sklearn** are used for utility tasks, i.e. train/valid split, target and track id loading etc.

Architecture of my model consists of 3 blocks:
- Transformer Encoder, which encodes input embeddings for knowledge extraction;
- 3 convolution blocks with different receptive fields for patterns extraction;
- MLP block for genre classification.

Average precision of trained model on validation subsample is 19 %.

Full code of my solution is available in **my-solution-yandex-cup-2023-recsys.ipynb** file in this repo.
