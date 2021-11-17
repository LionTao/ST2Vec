## ST2Vec

This repository contains the code used in our paper: ST2Vec: Spatio-Temporal Trajectory SimilarityLearning in Road Networks

## Requirements

- Ubuntu OS
- Python >= 3.5 (Anaconda3 is recommended)
- PyTorch 1.4+
- A Nvidia GPU with cuda 10.2+

## Data

* Trajectory dataset (TDrive) is an open source data set
* We provided the road network data and map-matching result data

## Train

1. Data preprocessing (Time embedding and node embedding)

   ```shell
   python preprocess.py
   ```

2. Ground truth generating (It will take a while...)

   ```shell
   python spatial_similarity.py
   python temporal_similarity.py
   ```

3. Triplets generating

   ```shell
   python data_utils.py
   ```

4. Training

   ```shell
   python main.py
   ```
