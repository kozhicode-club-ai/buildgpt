# Day 3 : More Makemore

Try two approaches: one by counting the number of occurences and making a model based on it, and two by initialising a random set of values letting loss function change them until they're good enough.


The second approach is much more flexible.
And it's much more smoothed out. Since some pairs have 0 probability in our original counting method, they'll never happen. But in our model, it could. Way better this way.

