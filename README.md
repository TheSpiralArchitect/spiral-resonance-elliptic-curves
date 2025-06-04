# 🌀 Spiral Resonance Law – Elliptic Curve Validation

This repository tests the **Spiral Resonance Law (SRL)** using Fourier coefficients from real elliptic curves. The SRL hypothesis proposes that analytic structure (such as rank) is encoded in spiral-phase interference patterns arising from a structured scalar field:

\[
\Phi(t) = \cos(\omega \log |t| + n \theta)
\]

We test whether elliptic curves of higher rank exhibit more **resonance nulls** — points where this field destructively interferes with the L-function signal — compared to random or Möbius-like controls.

---

## 🔍 What's in This Repo

- `srl_elliptic_curve_validation.ipynb`: Core notebook that runs the experiment, plots spiral interference, and compares null counts.
- **Null Summary Table:** Shows how $R_E(\epsilon)$ varies across rank 0–4 curves and control sequences.
- **Visualizations:** Includes field plots, absolute response overlays, and per-curve resonance patterns.

---

## 📐 Methods

### Spiral Field:
\[
\Phi(t) = \cos(\omega \log |t| + n \theta)
\]

- **ω** = 6.0: spiral frequency  
- **n** = 3: azimuthal mode  
- **ε** = threshold (e.g. 0.05–0.3) for resonance nulls  
- **Null** defined as:  
  \[
  |\Phi(t_n) \cdot a_n| < \epsilon
  \]

### Data:
- Curves: `11a1`, `37a1`, `389a1`, `5077a1`, `126484a1`  
- Ranks: 0–4 from LMFDB  
- Controls: Randomized $a_n$, Möbius μ(n)

---

## 📊 Results Summary

- **Higher-rank curves show more resonance nulls** at all thresholds tested.
- **Control tests** (random, Möbius) exhibit flat or inconsistent null profiles.
- Results support SRL's claim that analytic degeneracy (rank) manifests as increased spiral interference.

---

## 🧠 Interpretation

These results suggest a **resonant encoding** of elliptic curve rank within a logarithmic spiral phase structure. If validated across broader data, SRL could provide a novel lens on L-function behavior, spectral symmetry, and arithmetic geometry.

---

## 📎 Notes & Limitations

- $\theta$ is fixed at 0 throughout.  
- Only 5 real curves are tested (small sample).  
- $N = 50$ terms used; higher $N$ is possible.  
- Code is modular for adaptation to other domains.

## 📚 Citation & Use

If using this code or testing SRL in related work, please cite:

> **J. Patterson**, *Spiral Resonance Law – Elliptic Curve Validation*, GitHub, 2025.

---

## 🔭 Future Directions

- Add more elliptic curves with known rank and Fourier coefficients  
- Extend beyond N = 50 to test deeper L-function tails  
- Vary angular phase $\theta$ instead of fixing it at 0  
- Visualize 2D spiral embeddings and resonance landscapes  
- Test SRL on modular forms, Maass forms, or higher-genus $L$-functions  
- Compare null distributions to zero statistics in random matrix theory  

---

---

## ❓ What Is the Spiral Resonance Law?

The Spiral Resonance Law (SRL) proposes that emergent structure in mathematics and physics arises from alignment with a spiral scalar field:

$$
\Phi(t) = \cos(\omega \log |t| + n \theta)
$$

This log-periodic field models interference patterns observed in quasar distributions, quantum gates, EEG streams — and, in this notebook, elliptic curve $L$-functions. The number of resonance nulls — points where this spiral field nearly cancels the signal — is hypothesized to correlate with arithmetic complexity such as analytic rank.

---

## ✅ Summary

This repository provides a reproducible test of SRL on elliptic curves using real data, visual analysis, and randomized controls. All code is modular and extensible. Feedback, forks, and formal collaboration are welcome.

