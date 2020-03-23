# class_IDE

CLASS code for the "pure momentum transfer" coupled quintessence model first introduced in https://arxiv.org/abs/1307.0458 (the so-called "Type 3" theories in that paper). For more numerical results/plots also see https://arxiv.org/abs/1604.04222, https://arxiv.org/abs/1711.05196, and https://arxiv.org/abs/1912.09858. This version of the code is using the quadratic coupling function, $\beta Z^2$.

## Modifications to the code

The starting point is the uncoupled quintessence CLASS implementation. The coupling effects are parameterised by "scf_veta" (the $\beta$ in the quadratic coupling function assumed). If this is set to 0, the code is uncoupled quintessence. For more details on the equations, the quadratic coupling function, the quintessence potential used etc., see Pourtsidou & Tram https://arxiv.org/abs/1604.04222. The coupling implementation has been done in input.c, background.c, and perturbations.c.

