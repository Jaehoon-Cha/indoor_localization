- [2017-08-13](#org72d7e2d)
- [2017-08-12](#org13de1d1)

This is a repository for research on indoor localization based on wireless fingerprinting techniques. For more details, please visit [XJTLU SURF project home page](http://kyeongsoo.github.io/research/projects/indoor_localization/index.html).


<a id="org72d7e2d"></a>

# 2017-08-13

We [replace the activation functions of the hidden-layer from 'tanh' to 'relu'](./python/indoor_localization-2.ipynb) per the second answer to [this qustion](https://stats.stackexchange.com/questions/218542/which-activation-function-for-output-layer). The results are [here](./results/indoor_localization-2_20170813.csv) (nh: number of hidden layer nodes, dr: dropout rate, acc: accuracy). Compared to the case with 'tanh', however, the results seem to not improve (a bit inline with the gut-feeling suggestions from [this](https://datascience.stackexchange.com/questions/10048/what-is-the-best-keras-model-for-multi-class-classification)).


<a id="org13de1d1"></a>

# 2017-08-12

We first try [a feed-forward classifier with just one hidden layer](./python/indoor_localization-1.ipynb) per the comments from [this](https://stats.stackexchange.com/questions/181/how-to-choose-the-number-of-hidden-layers-and-nodes-in-a-feedforward-neural-netw). The results are [here](./results/indoor_localization-1_20170812.csv) (\* *nh*: number of hidden layer nodes, *dr*: [dropout](https://en.wikipedia.org/wiki/Dropout_(neural_networks)) rate, *loss*: [categorical cross-entropy](http://deeplearning.net/software/theano/library/tensor/nnet/nnet.html#theano.tensor.nnet.nnet.categorical_crossentropy), *acc*: accuracy \*).
