# American sign language
This project has been created to train a model and then predict the outcomes based on that model.


## Requirement
1. python 3.7
2. install anaconda and create a virtual environment
3. install all mentioned libraries in file (requirement)


## Dataset
download datasets from kaggle.com 
## How to use
### Using nn
1. run train_simple_nn.py file using this commad
`python train_simple_nn.py --dataset animals --model output/simple_nn.model \
	--label_bin output/simple_nn_lb.pickle --plot output/simple_nn_plot.png`

2. run predict.py file using this command
`python predict.py --image images/cat.jpg --model output/simple_nn.model \
	--label_bin output/simple_nn_lb.pickle --width 32 --height 32 --flatten 1`

### Using cnn
1. run train_vgg.py file using this command `python train_vgg.py --dataset animals --model output/smallvggnet.model \
	--label_bin output/smallvggnet_lb.pickle \
	--plot output/smallvggnet_plot.png`
2. run predict.py file `python predict.py --image images/panda.jpg --model output/smallvggnet.model \
	--label_bin output/smallvggnet_lb.pickle --width 64 --height 64`
