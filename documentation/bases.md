---
layout: post
title: Bases
math: true
author: Alpaca
toc: true
---


## Bases above the EW scale

### Derivative basis

* **Name:** ```derivative_above```
* **Lagrangian:**

$$
\mathcal{L} \subset \frac{a}{f_a}\left(\frac{g_B^2}{16\pi^2} c_{B}B_{\mu\nu}\tilde{B}^{\mu\nu} + \frac{g_W^2}{16\pi^2}c_{W} W^i_{\mu\nu}\tilde{W}^{i,\mu\nu}+\frac{g_s^2}{16\pi} c_{g}G^a_{\mu\nu}\tilde{G}^{a,\mu\nu}\right) + \frac{\partial^\mu a}{f_a} \left(\bar{q}_L c_{q_L} \gamma_\mu q_L  + \bar{u}_R c_{u_R} \gamma_\mu u_R + \bar{d}_R c_{d_R} \gamma_\mu d_R + \bar{\ell}_L c_{\ell_L} \gamma_\mu \ell_L + \bar{e}_R c_{e_R} \gamma_\mu e_R \right)
$$

* **Parameters:**
  * ```cB```: Coupling to $B$ bosons $c_B$, ```float```.
  * ```cW```: Coupling to $W$ bosons $c_W$, ```float```.
  * ```cg```: Coupling to gluons $c_g$, ```float```.
  * ```cqL```: Coupling to left-handed quarks $c_{q_L}$, $3\times 3$ ```numpy.matrix```.
  * ```cuR```: Coupling to right-handed up-type quarks $c_{u_R}$, $3\times 3$ ```numpy.matrix```.
  * ```cdR```: Coupling to right-handed down-type quarks $c_{d_R}$, $3\times 3$ ```numpy.matrix```.
  * ```clL```: Coupling to left-handed leptons $c_{\ell_L}$, $3\times 3$ ```numpy.matrix```.
  * ```ceR```: Coupling to right-handed charged leptons $c_{e_R}$, $3\times 3$ ```numpy.matrix```.
* **Notes:**
  * Fermions are weak eigensates.
* **References:**
  * Equation (1) of M. Bauer, M. Neubert, S. Renner, M. Schnubel, A. Tham: _The Low-Energy Effective Theory of Axions and ALPs_. JHEP 04 (2021) 063. [DOI](https://doi.org/10.1007/JHEP04(2021)063), [arXiv](https://arxiv.org/abs/2012.12272).

### Mass basis

* **Name:** ```massbasis_above```
* **Lagrangian:**

$$
\mathcal{L} \subset \frac{a}{f_a}\left(\frac{\alpha_\mathrm{em}}{4\pi}c_{\gamma} F_{\mu\nu}\tilde{F}^{\mu\nu} + \frac{\alpha_\mathrm{em}}{2\pi s_w c_w}c_{\gamma Z} F_{\mu\nu}\tilde{Z}^{\mu\nu} + \frac{\alpha_\mathrm{em}}{4\pi s_w^2 c_w^2}c_{Z} Z_{\mu\nu}\tilde{Z}^{\mu\nu} + \frac{\alpha_\mathrm{em}}{2\pi s_w^2}c_{W} W^+_{\mu\nu}\tilde{W}^{-\mu\nu} + \frac{\alpha_s}{4\pi}c_{g} G^a_{\mu\nu}\tilde{G}^{a,\mu\nu}\right) + \frac{\partial^\mu a}{f_a} \left(\bar{u}_L k_U \gamma_\mu u_L  + \bar{u}_R k_u \gamma_\mu u_R + \bar{d}_L k_D \gamma_\mu d_L + \bar{d}_R k_d \gamma_\mu d_R + \bar{e}_L k_E \gamma_\mu e_L + \bar{e}_R k_e \gamma_\mu e_R + \bar{\nu}_L k_\nu \gamma_\mu \nu_L \right)
$$

* **Parameters:**
  * ```cgamma```: Coupling to photons $c_\gamma$, ```float```.
  * ```cgammaZ```: Coupling to photon and $Z$ boson $c_{\gamma Z}$, ```float```.
  * ```cZ```: Coupling to $Z$ bosons $c_Z$, ```float```.
  * ```cW```: Coupling to $W$ bosons $c_W$, ```float```.
  * ```cg```: Coupling to gluons $c_g$, ```float```.
  * ```kU```: Coupling to left-handed up-type quarks $k_U$, $3\times 3$ ```numpy.matrix```.
  * ```ku```: Coupling to right-handed up-type quarks $k_u$, $3\times 3$ ```numpy.matrix```.
  * ```kD```: Coupling to left-handed down-type quarks $k_D$, $3\times 3$ ```numpy.matrix```.
  * ```kd```: Coupling to right-handed down-type quarks $k_d$, $3\times 3$ ```numpy.matrix```.
  * ```kE```: Coupling to left-handed charged leptons $k_E$, $3\times 3$ ```numpy.matrix```.
  * ```ke```: Coupling to right-handed charged leptons $k_e$, $3\times 3$ ```numpy.matrix```.
  * ```kNu```: Coupling to left-handed neutrinos $k_\nu$, $3\times 3$ ```numpy.matrix```.
* **Notes:**
  * Fermions are mass eigensates.
* **References:**
  * Equations (39) and (43) of M. Bauer, M. Neubert, S. Renner, M. Schnubel, A. Tham: _The Low-Energy Effective Theory of Axions and ALPs_. JHEP 04 (2021) 063. [DOI](https://doi.org/10.1007/JHEP04(2021)063), [arXiv](https://arxiv.org/abs/2012.12272).


## Bases below the EW scale

### $k_F$ basis

* **Name:** ```kF_below```
* **Lagrangian:**

$$
\mathcal{L} \subset \frac{a}{f_a}\left(\frac{\alpha_\mathrm{em}}{4\pi}c_{\gamma} F_{\mu\nu}\tilde{F}^{\mu\nu} + \frac{\alpha_s}{4\pi}c_{g} G^a_{\mu\nu}\tilde{G}^{a,\mu\nu}\right) + \frac{\partial^\mu a}{f_a} \left(\bar{u}_L k_U \gamma_\mu u_L  + \bar{u}_R k_u \gamma_\mu u_R + \bar{d}_L k_D \gamma_\mu d_L + \bar{d}_R k_d \gamma_\mu d_R + \bar{e}_L k_E \gamma_\mu e_L + \bar{e}_R k_e \gamma_\mu e_R + \bar{\nu}_L k_\nu \gamma_\mu \nu_L \right)
$$

* **Parameters:**
  * ```cgamma```: Coupling to photons $c_\gamma$, ```float```.
  * ```cg```: Coupling to gluons $c_g$, ```float```.
  * ```kU```: Coupling to left-handed up-type quarks $k_U$, $2\times 2$ ```numpy.matrix```.
  * ```ku```: Coupling to right-handed up-type quarks $k_u$, $2\times 2$ ```numpy.matrix```.
  * ```kD```: Coupling to left-handed down-type quarks $k_D$, $3\times 3$ ```numpy.matrix```.
  * ```kd```: Coupling to right-handed down-type quarks $k_d$, $3\times 3$ ```numpy.matrix```.
  * ```kE```: Coupling to left-handed charged leptons $k_E$, $3\times 3$ ```numpy.matrix```.
  * ```ke```: Coupling to right-handed charged leptons $k_e$, $3\times 3$ ```numpy.matrix```.
  * ```kNu```: Coupling to left-handed neutrinos $k_\nu$, $3\times 3$ ```numpy.matrix```.
* **References:**
  * Equations (54) and (43) of M. Bauer, M. Neubert, S. Renner, M. Schnubel, A. Tham: _The Low-Energy Effective Theory of Axions and ALPs_. JHEP 04 (2021) 063. [DOI](https://doi.org/10.1007/JHEP04(2021)063), [arXiv](https://arxiv.org/abs/2012.12272).

### Vector-axial basis

* **Name:** ```VA_below```
* **Lagrangian:**

$$
\mathcal{L} \subset \frac{a}{f_a}\left(\frac{\alpha_\mathrm{em}}{4\pi}c_{\gamma} F_{\mu\nu}\tilde{F}^{\mu\nu} + \frac{\alpha_s}{4\pi}c_{g} G^a_{\mu\nu}\tilde{G}^{a,\mu\nu}\right) + \frac{\partial^\mu a}{2f_a} \left(\bar{u} \gamma_\mu (c_u^V + c_u^A \gamma_5) u + \bar{d} \gamma_\mu (c_d^V + c_d^A \gamma_5) d + \bar{e} \gamma_\mu (c_e^V + c_e^A \gamma_5) e + 2\bar{\nu}_L c_\nu \gamma_\mu \nu_L \right)
$$

* **Parameters:**
  * ```cgamma```: Coupling to photons $c_\gamma$, ```float```.
  * ```cg```: Coupling to gluons $c_g$, ```float```.
  * ```cuV```: Vectorial coupling to up-type quarks $c_u^V$, $2\times 2$ ```numpy.matrix```.
  * ```cuA```: Axial coupling to up-type quarks $c_u^A$, $2\times 2$ ```numpy.matrix```.
  * ```cdV```: Vectorial coupling to down-type quarks $c_d^V$, $3\times 3$ ```numpy.matrix```.
  * ```cdA```: Axial coupling to down-type quarks $c_d^A$, $3\times 3$ ```numpy.matrix```.
  * ```ceV```: Vectorial coupling to charged leptons $c_e^V$, $3\times 3$ ```numpy.matrix```.
  * ```ceA```: Axial coupling to charged leptons $c_e^A$, $3\times 3$ ```numpy.matrix```.
  * ```cnu```: Coupling to left-handed neutrinos $c_\nu$, $3\times 3$ ```numpy.matrix```.
