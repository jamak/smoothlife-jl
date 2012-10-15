#smoothlife-jl

##An implementation of the [SmoothLife](http://arxiv.org/abs/1111.1567) algorithm in Julia

The project is super rough at this point, since I'm not even sure which Julia graphics library to use,(or even which actually works) but I am reasonably positive that the algorithm works as described in the paper.

###How exactly is that, exactly?

Glad you asked. This algorithm generalizes [Conway's Game of Life](http://en.wikipedia.org/wiki/Conway's_Game_of_Life) to a continuous domain by replacing the rules with continuous analogues. In the discrete GoL the state of a cell for the next timestamp can be determined by the current live-state of the cell (0 or 1) and the number of living neighbors, which could be between 0 or 8. Hence, the state could be described with a 2x9 matrix containing all possible combinations. Instead of such a transition matrix, we have a transition function s(m,n) which determines possible states. I can't say much more without block-quoting the paper, and it really is quite short and worth reading.
