# Multi-objective_optimization
This sample code is trying to find Pareto front using PHYSBO, targeting 3 glass properties at the same time with visuals like a responsive surface. The notebook [3] is computing Pareto front, and from [1] to [2] are just preparation for [3]. The dataset is from the public SciGlass; targets are modulus, density, and Tg. Regression models are all random forest with hyperparameter tuning. PHYSBO has multiple options to compute Pareto front: random search, Bayesian optimization (BO), and full search, and this example uses BO. The red dots in the first graph are Pareto front. The second graph shows fitted surface with Pareto front, but the surface is made by kernel Ridge regression (kernel = "poly") just to help see the front curve, so this is a simple approximation and no physical meaning.

![Pareto_front_example](https://user-images.githubusercontent.com/50325966/160373983-31bf1763-318d-4238-b932-1fb74744cc60.jpg)

![pred_surface](https://user-images.githubusercontent.com/50325966/160374262-36e1d1a9-e2d1-412f-ad21-fc202d2f5294.jpg)
