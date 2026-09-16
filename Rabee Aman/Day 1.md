## Today's Task
Building Micrograd

What's micrograd? 

A. It's a neural network library much simpler version of pytorch.

Backpropagation (as I know rn): 
go backwards from the output to get the gradient value of the first values. Basically find out how a and b affect a variable g down the line.

Micrograd is the most basic thing to build.. and basically all you need to train neural networks.

What's a derivative?
It's a value that shows how much something changes when something else changes.

Why a value class, and not just a value? 

A. Because value by itself can't contain any information on how it was made or what its derivative is. For backpropagation we need classes to store gradients.

How derivative changes according to the operator when propagating backwards:

when operator is '+', derivative is just carried over from sum to operands.
when operator is (*), derivative is grad of product multiplied by the value of the OTHER operand.

use chain rule-- generally.

What's loss?

It's a value that tells you how off you are from the desired output. 

Fixing loss: 
1. find loss
2. use backpropagation to find how much each value contributes to loss. 
3. adjust each value slightly in favour of decreasing loss
4. run it again.



