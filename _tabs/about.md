---
# the default layout is 'page'
icon: fas fa-info-circle
order: 6
math: true
---

**ALP-ACA:** the ALP Automated Computing Algorithm

> This site is under construction
{: .prompt-warning }

## Introduction to ALPs

Axion-Like Particles (ALPs) are one of the most popular examples of physics beyond the Standard Model (SM) of particle physics. They are light pseudoscalar particles that arise as the pseudo-Nambu Goldstone boson of some spontaneously broken global $U(1)$ symmetry, and as such, are predicted in a wide range of New Physics models. The difference between ALPs and QCD axions is that in the former case, the mass of the pseudoscalar, $m_a$, and the energy scale at which the symmetry spontaneously breaks, $f_a$, are independent parameters, while in the latter case they are constrained by the relation $m_a f_a \approx m_\pi f_\pi$. As a result, ALPs are viable in a much wider range of masses, including those in the reach of particle colliders.

### New Physics: Light or heavy?

[Comments about different signatures. Heavy NP can be studied in a model-independent way with EFTs, while light NP requires a case-by-case analysis]

### Solving the Universe with ALPs

The growing interest in ALPs resides in their ability, depending on the values of $m_a$ and $f_a$ considered, to solve or alleviate some of the long-standing questions afflicting particle physics:

* The strong CP problem, through the Peccei-Quinn mechanism. Strong interactions do not exhibit any violation of the CP symmetry, as evidenced by the null value, to great experimental accuracy, of the electric dipole moment of the neutron. According to the Peccei-Quinn mechanism, an axion would naturally drive the CP-violating parameter of the strong interaction, $\theta_\mathrm{QCD}$, to zero.
* Linked to the violation of the CP symmetry there is the problem of baryogenesis, or why there is an imbalance between matter and antimatter in the Universe. One of the Sakharov conditions for baryogenesis is precisely a sizable violation of the CP symmetry, and the CP violation observed in electroweak quark processes is not enough to explain the imbalance between matter and anti-matter.
* Light axions or ALPs could be a component of the cold Dark Matter, that according to the current cosmological models ($\Lambda$-CDM) constitutes nearly 27% of the energy content of our Universe.
* Neutrinos are known to have small but non-zero masses (or more precisely, at least two of the neutrino species). However, the mechanism generating those masses is currently unknown. The seesaw mechanism explains the tiny neutrino masses as being inversely proportional to the large masses of the sterile right-handed Majorana neutrinos. The sterile neutrinos would receive their masses through the spontaneous breaking of a global $U(1)$ symmetry, thus the associated Goldstone boson, dubbed as Majoron, is a special case of ALP.
* Flavour puzzle
* A(n)dd more...

### Playing hide-and-seek with ALPs

[List and comment on the various experimental signatures: cosmology, astrophysics, helioscopes, light-through-walls, beam dumps, colliders, etc,]

## The role of ALP-ACA

[Compare to the situation of heavy NP physics, with consolidated codes: flavio, eos, HEPfit. Shutout to Ciaran O'Hare and his repository]

### Our goals

* Creating a database of UV models that produce ALP (e.g. DFSZ, KSVZ), and implementation of their matching into the ALP Lagrangian.
* Implementating the full one-loop running of the ALP Lagrangian. Extending the results of Bauer, Neubert et al to contributions which are not proportional to the top Yukawa, and cross-checking with automatic matching tools like MatchMakerEFT or Matchete.
* Creating a database of the different bases of ALP operators used in the literature, and a tool to translate between them.
* Calculating all decay channels of the ALP, with special focus on the hadronic decays in the 1-3 GeV range, which are notoriously difficult. In this respect, we are extending Aloni's framework to include also ALP couplings to quarks.
* Calculating production cross-sections for ALPs in colliders like BaBar, Belle, Belle II, BESIII and LHC, in processes like quarkonia decays and leptonic, semileptonic, hadronic and radiative meson decays. We will include the interplay between the lifetime of the ALP and the size of the detectors, resulting in the different regimes of prompt decays, decays with resolved displaced vertices or invisible decays.
* Creating and update of a database for the experimental measurements relevant for the processes calculated with our code.
* Performing statistical analysis to determine exclusion regions and fits of the parameters, combining the theoretical calculations and the experimental data.
* Keeping track of the references to all the formulas and experimental values used during the use of the code, and generating 
* In future stages of the development, more observables will be included in the code: anomalous magnetic moments, LFV observables, astrophysical probes, cosmology, helioscopes, etc.

The end goal is to provide a one-size-fits-all code such that the user provides a Lagrangian, and with a few lines of code, will obtain a complete picture of the excluded and favoured parameters of their model.
As the name suggests, a true ALP Automated Computed Algorithm (and also a cool acronym! 🦙).
