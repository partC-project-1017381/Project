# Final-Year-Project-1017381
This is the Github repository that contains code for the Part-c Project of candidate 1017381 


# Abstract
Recent studies have shown that state-of-the-art Optical Character Recognition (OCR) deep learning models are vulnerable to adversarial attacks. In this work, we provide robustness guarantees for OCR neural networks which comprise of convolution layers to obtain spatial features and recurrent layers to capture relations between frames. In particular, we study the Maximum Safe Radius problem, which computes the minimum distance to an adversarial example given an input sample, and the Feature Robustness problem, which gives comparisons of robustness against adversarial perturbation between features of an input sample. We show that when provided with the Lipschitz constant of the network, this problem can be approximated with guarantees using finite optimisation by discretizing the input space. This optimisation problem can be solved using a two-player turn-based game where the first player chooses a feature and the second player imposes a perturbation within that feature. We also exploit output range analysis methods to compute a lower bound of the Maximum Safe Radius and draw comparisons between the two robustness certification methods. Furthermore, we investigate methods to estimate the Lipschitz constants and evaluate how better bounds for the Lipschitz constant affect the performance of the game-based algorithm. Finally, experiments and evaluations are conducted on the ICDAR13 dataset.

# Developer's Platform
```
python 3.6
tensorflow-gpu 2.1.0
numpy 1.18.1
opencv 4.2.0
matplotlib 3.1.3
```

# Run
Code for training the network and the trained model are in NeuralNetwork.

Code for the game-based method is in DeepGame.

Code for Lipschitz constant estimation is in Lipschitz, where CLEVER is the extreme value approach, and rnn_bound, cnn_bound are output range analysis approaches.

The training and test datasets are in data.

