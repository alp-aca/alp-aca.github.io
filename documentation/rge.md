---
layout: post
title: Renormalization Group Evolution
math: true
author: Alpaca
toc: true
---

Alpaca implements the running of the ALP couplings and the matching to the low-energy Lagrangian (i.e. with $W^\pm$, $Z$ and $t$ integrated out) as described in [^1].

The following code exemplifies the running between the scale $\mu= 1000\,\mathrm{GeV}$ down to $\mu= 5\,\mathrm{GeV}$, using the method `match_run`:

```python
from alpaca import ALPcouplings

couplings_high = ALPcouplings({'cqL': 1.0}, scale=1000, basis='derivative_above')
couplings_low = couplings_high.match_run(scale=5, basis='VA_below')
```

The method `match_run` takes the following arguments:

- `scale` [```float```]: energy scale of the final couplings. Must be smaller than the initial scale.
- `basis` [`str`]: basis of the final couplings, as described [here](bases).
- `integrator` [`str` optional, default `'scipy'`]: Method used to numerically integrate the RG equations. The available options are

  - `scipy`: Solves the initial value problem given by

  $$
  \frac{d c_i(\mu)}{d \log \mu} = \frac{1}{16\pi^2} \gamma_{ij}(\mu) c_j(\mu)\,;\qquad c_i(\mu = \Lambda)=c_i^0\,,
  $$

  using the Runge-Kutta integrator implemented by [scipy](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
  - `leadinglog`: In the expression above, by approximating $\gamma_{ij}(\mu)$ as a constant (i.e. by neglecting the running of the SM parameters), an approximate solution can be found as 
  
  $$
  c_i(\mu) \approx \left(\delta_{ij} + \frac{\gamma_{ij}}{16\pi^2}\log\frac{\mu}{\Lambda} \right)c_j(\Lambda)\,,
  $$
  
  which can be computed efficiently as a matrix multiplication.
  - `no_rge`: Does not change the values of the couplings, and just modifies the scale.
- `beta` [`str` optional, default `full`]: Controls the expression of the $\beta$ functions used for the running:

  - `ytop`: discards all the terms proportional to the Yukawa couplings other than $y_t$.
  - `full`: retains the full dependency on all the Yukawa couplings.
- `matching_scale` [`float`, default `100`]: Energy where the matching between the full ALP Lagrangian and the low-energy Lagrangian is performed.
- `match_2loops` [`bool`, default `False`]: whether or substitute the 1-loop effective gauge couplings in the 1-loop matching expression.

## References

[^1]: M. Bauer, M. Neubert, S. Renner, M. Schnubel, A. Thamm: "The Low-Energy Effective Theory of Axions and ALPs". JHEP 04 (2021), 063. [arXiv:2012.12272 [hep-ph]](https://arxiv.org/abs/2012.12272)
