
Here the class of functions is controlled by explicitly penalizing RSS(f ) with a roughness penalty

PRSS(f;λ) = RSS(f) +λJ(f).     (2.38) 

The user-selected functional J(f) will be large for functions f that vary too rapidly over small regions of input space. 
For example, the popular cubic smoothing spline for one-dimensional inputs is the solution to the penalized least-squares 
criterion 

PRSS(f;λ ) =N X i =1 (yi−f(xi))2+ λZ [f′′(x)]^2 dx. v(2.39) 

The roughness penalty here controls large values of the second
derivative off, and the amount of penalty is dictated byλ≥0. Forλ = 0 no penalty is imposed, and any interpolating function will
do, while forλ=∞ only functions linear inx are permitted. Penalty functionalsJ can be constructed for functions in any dimension,
and special versions can be created to impose special structure. For ex-ample, additive penaltiesJ(f) =P p j=1J(fj ) are used in
conjunction with additive functionsf(X) =P p j=1fj(Xj ) to create additive models with smooth coordinate functions. Similarly,projection pursuit regression mod-els havef(X) =P M m=1gm(αTmX) for adaptively chosen directionsαm , and the functionsgm can
each have an associated roughness penalty. Penalty function, orregularization methods, express our prior belief that the type of
functions we seek exhibit a certain type of smooth behavior, and indeed can usually be cast in a Bayesian framework. The penaltyJ
corre-sponds to a log-prior, and PRSS(f;λ ) the log-posterior distribution, and minimizing PRSS(f;λ ) amounts to finding the
posterior mode. 
We discuss roughness-penalty approaches in Chapter 5 and the Bayesian paradigm in Chapter 8.
