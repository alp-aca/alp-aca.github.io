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

Axion-Like Particles (ALPs) represent a significant and widely studied extension of the Standard Model (SM) in particle physics. ALPs are light pseudoscalar particles that emerge as pseudo-Nambu-Goldstone bosons resulting from the spontaneous breaking of a global $U(1)$ symmetry. ALPs are theoretically predicted within various New Physics models. A key distinction between ALPs and Quantum Chromodynamics (QCD) axions lies in the relationship between their mass $m_a$) and the symmetry-breaking energy scale ($f_a$). In the case of ALPs, these two parameters are independent, whereas in QCD axions, they are related by the constraint $m_a f_a \approx m_\pi f_\pi$. This independence allows ALPs to be viable across a broader range of mass scales, including those accessible to particle collider experiments.

### New Physics: Light or heavy?

[Comments about different signatures. Heavy NP can be studied in a model-independent way with EFTs, while light NP requires a case-by-case analysis]

### Solving the Universe with ALPs

The increasing interest in Axion-Like Particles (ALPs) stems from their potential to address or mitigate several long-standing issues in particle physics, depending on the specific values of $m_a$ and $f_a$ considered. These issues include:

- **The strong CP problem**, which may be resolved through the Peccei-Quinn mechanism. Despite theoretical predictions, strong interactions exhibit no violation of CP symmetry, as evidenced by the experimentally observed null value of the neutron's electric dipole moment. The Peccei-Quinn mechanism posits that the axion would naturally drive the CP-violating parameter in QCD, $\theta_\mathrm{QCD}$, to zero.
  
- **The baryogenesis problem**, linked to CP symmetry violation, refers to the observed imbalance between matter and antimatter in the Universe. According to the Sakharov conditions, a significant violation of CP symmetry is required for baryogenesis, yet the CP violation observed in electroweak quark processes is insufficient to explain the matter-antimatter asymmetry.

- **Dark Matter**: Light axions or ALPs could constitute a portion of cold dark matter, which, according to the current cosmological model ($\Lambda$-CDM), accounts for nearly 27% of the total energy content of the Universe.

- **Neutrino mass**: Although neutrinos are known to have small but non-zero masses (with at least two species exhibiting mass), the mechanism responsible for generating these masses remains unclear. The seesaw mechanism explains the small neutrino masses as inversely proportional to the large masses of sterile right-handed Majorana neutrinos. These sterile neutrinos are thought to acquire their masses through the spontaneous breaking of a global $U(1)$ symmetry, with the associated Goldstone boson, called the Majoron, being a specific case of an ALP.

* Flavour puzzle
* A(n)dd more...

### Playing hide-and-seek with ALPs

[List and comment on the various experimental signatures: cosmology, astrophysics, helioscopes, light-through-walls, beam dumps, colliders, etc,]

## The role of ALP-ACA

[Compare to the situation of heavy NP physics, with consolidated codes: flavio, eos, HEPfit. Shout-out to Ciaran O'Hare and his repository]

### Our goals

The objectives of our project are outlined as follows:

- **Developing a comprehensive database of UV models** that generate ALPs, such as DFSZ and KSVZ models, and implementing their matching to the ALP effective Lagrangian.
  
- **Implementing the full one-loop renormalization group running** of the ALP effective Lagrangian. This includes extending the results of Bauer, Neubert, et al., to contributions beyond those proportional to the top Yukawa coupling, and cross-checking these results with automated matching tools like MatchMakerEFT or Matchete.
  
- **Creating a database of ALP operator bases** commonly used in the literature and developing a tool to facilitate translations between different bases.

- **Calculating all ALP decay channels**, with a particular focus on the challenging hadronic decays in the 1-3 GeV mass range. In this regard, we are extending Aloni's framework to incorporate ALP-quark couplings.

- **Calculating production cross-sections for ALPs** in collider experiments such as BaBar, Belle, Belle II, BESIII, and the LHC. These calculations will cover a variety of processes, including quarkonia decays, and leptonic, semileptonic, hadronic, and radiative meson decays. Special attention will be given to the interplay between the ALP lifetime and the detector sizes, leading to different regimes of prompt decays, decays with displaced vertices, and invisible decays.

- **Maintaining and updating a database of experimental measurements** relevant to the processes calculated by our code.

- **Performing statistical analyses** to derive exclusion regions and parameter fits by combining our theoretical calculations with experimental data.

- **Tracking references for all formulas and experimental values** used in the code, with automatic generation of records in BibTeX format.

- **In future development stages**, the code will be expanded to include additional observables such as anomalous magnetic moments, lepton flavor-violating (LFV) observables, astrophysical probes, cosmological data, helioscopes, and more.

The end goal is to provide a one-size-fits-all code such that the user provides a Lagrangian, and with a few lines of code, will obtain a complete picture of the excluded and favoured parameters of their model.
As the name suggests, a true ALP Automated Computed Algorithm (and also a cool acronym! 🦙).
