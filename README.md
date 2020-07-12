# class_IDE 
### based on CLASS v2.9.3

This repository contains the CLASS code for the "pure momentum transfer" coupled quintessence model first introduced in [Pourtsidou, Skordis and Copeland](https://arxiv.org/abs/1307.0458) (the so-called "Type 3" theories in that paper). For numerical results/plots also see [Pourtsidou and Tram](https://arxiv.org/abs/1604.04222), [Linton et al.](https://arxiv.org/abs/1711.05196), and [Chamings et al.](https://arxiv.org/abs/1912.09858). This version of the code is using the quadratic coupling function, $\beta Z^2$, which was shown to fit data very well in [Pourtsidou and Tram](https://arxiv.org/abs/1604.04222) and be able to alleviate the σ8 "tension".

## Modifications to the code to include the momentum transfer coupling

The starting point is the uncoupled quintessence CLASS implementation. The coupling effects are parameterised by a constant parameter `scf_veta` (the $\beta$ coupling parameter in the quadratic coupling function assumed). If this is set to 0, we recover the uncoupled quintessence case. For more details on the equations, the quadratic coupling function, the quintessence potential used etc., see [Pourtsidou and Tram](https://arxiv.org/abs/1604.04222). 

For more details on the coupling implementation in this code, see the modifications in `input.c, `background.h`, background.c, and perturbations.c` (search for `scf_veta`). The test run file is `IDE_parameters.ini`, so you need to compile and then do `./class IDE_parameters.ini`. 
