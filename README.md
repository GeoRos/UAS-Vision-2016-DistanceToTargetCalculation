# UAS-Vision-2016-DistanceToTargetCalculation

Fully-Connected Neural Net to calculate the horizontal distance to the target (MATLAB)

This code trains a Fully-Connected Neural Network to be able to calculate the horizontal distance from the UAV to the target as described by the IMechE Competition's Target Description (https://www.imeche.org/get-involved/young-members-network/auasc). The network is currently trained to be able to calculate the distance with an accuracy of 93.6% using as inputs the roll-angle and the altitude of the aircraft and the position of the observed target on the image.

The network is based on the Convolution Neural Network produced after finishing the Stanford UFLDL Tutorial (http://ufldl.stanford.edu/tutorial/), although it has been changed a lot.

INSTRUCTIONS Begin the program by running the fcTrain script. The network characteristics can be changed from the same script. The optimumThetaFC.mat file contains the optimum parameters required to achieve 93.6% accuracy. In order for these parameters to work the network needs to have the following characteristics:

input dimension   : 5
number of classes : 1 
fully-connected layer sizes: [100, (number of classes)]

If training of a new network is required, make sure to first copy the current optimum parameters to another directory since they will be overwritten as soon as training finishes
