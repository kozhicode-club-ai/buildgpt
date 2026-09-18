Day 1

BackPropoagtion: Going Backwards to from the last node to figure out how we could improve on      the solution that were given during the claculation. 


Micrograd a basic version of pytorch

a lot of explaining derivatives

during backpropogation we use gradiesnt which are derivatives of that current node wrt to the final result, it tells by how much we should increase or decrease the weight until the local minima is reached or when the validation performance begins to reduce, because of overfitting(learning the training data too well, it memorizes random noises and outliers)

to find the gradietn we use chain rule
when (+) gradient is the saem as the gradient of the child
when (*) gradient is the same as the otehr parent

LOSS: it is how wrong your answer is compared to the target answer 
Gradient: Which direction to move each weight, and how sensitive the error is to small changes in each weight.