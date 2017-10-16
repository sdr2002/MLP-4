# MLP-4
Assignment 4 for Deep Learning Practical course at University of Edinburgh: MSD-10 classification

1) Environment: Anaconda build is recommended
- python 2.7
- tensorflow 1.0
- numpy, matplotlib
- ipython, jupyter

2) Models: I lost convolved-GRU codes but will upload I found them back from the university server
- vRNN baseline
- LSTM or GRU baseline
- CNN baseline
- Convolved-GRU: TBA
- Convolved-Highway network-Bidirectional GRU: TBA

3) Summary of the report:
- In terms of validation set accuracy, GRU (also stable) > LSTM >> vanilla RNN
- Dropout wrapping works for gated-RNNs when the networks goes deeper(>2 layers), but L^n regularisation also works
- CNN baed embedding without dropout boosts the performace of GRU classifier
- Attention mechanism does not work: it is not quite obvious as because the task was about classification
- Sequential autoencoding does not help
- Optimise to classify in every time-step > last time-step, however over-fit occurs and L^n regularisation does not alleviate.
- Bidirectional GRU which the backward GRU optimises the first-half of the sequence and the forward GRU optimises the second-half alleviates the above over-fitting.
