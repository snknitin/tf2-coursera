# tf2-coursera
Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning


The simplest possible neural network is one that has only one neuron in it, and that's what this line of code does. In keras, you use the word dense to define a layer of connected neurons. There's only one dense here. So there's only one layer and there's only one unit in it, so it's a single neuron. Successive layers are defined in sequence, hence the word sequential. But as I've said, there's only one. So you have a single neuron. You define the shape of what's input to the neural network in the first and in this case the only layer, and you can see that our input shape is super simple. It's just one value.

        model = keras.Sequential([])


The neural network has no idea of the relationship between X and Y, so it makes a guess. Say it guesses Y equals 10X minus 10. It will then use the data that it knows about, that's the set of Xs and Ys that we've already seen to measure how good or how bad its guess was. The loss function measures this and then gives the data to the optimizer which figures out the next guess. So the optimizer thinks about how good or how badly the guess was done using the data from the loss function. Then the logic is that each guess should be better than the one before. As the guesses get better and better, an accuracy approaches 100 percent, the term convergence is used. In this case, the loss is mean squared error and the optimizer is SGD which stands for stochastic gradient descent
