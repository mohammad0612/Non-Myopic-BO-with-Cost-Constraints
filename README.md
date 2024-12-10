# Non-Myopic-BO-with-Cost-Constraints

Bayesian Optimization (BO) is a powerful tool for optimizing expensive black-box
functions. It treats the objective function as a probabilistic model and iteratively
updates this model based on observations, typically using Gaussian Processes (GPs).
Bayesian optimization can be used in a setting where evaluation is expensive, say
tuning the parameters of a neural network to optimize accuracy. Consider the
scenario where each evaluation point has a cost associated to it, and there is a
budget of the total cost to optimize the underlying function. Say this cost is
unknown a-priori and it must be explored as the objective function is evaluated.
This is the setting this paper will explore and propose a methodology to model such
a scenario by building a GP around both the cost function and objective function.
