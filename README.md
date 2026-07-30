# FNO(Fourier Neural Operator) - 'Fourier Neural Operator for Parametric Partial Differential Equations'
Utilizing Fourier transformaion to reduce calculating cost for high-dimensional problem is main idea in FNO.
The NN(Neural Network) in this method consist of three parts.

First, lifting layer which lift dimension of input data to higher dimension.
Second, Fourier layer which conduct Fourier transformation and calculate gradient to get clue for approximate solution. Basically use three Fourier layers for learning.
Third, projection layer which maps the output of the Fourier layers back to the original low-dimensional space.

Usually, the number of Fourier modes, which represents the number of frequency components retained after the Fourier transform is the main hyperparameter in the training process.
