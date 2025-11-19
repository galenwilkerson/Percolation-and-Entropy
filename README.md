# Percolation and Entropy

A Visual and Interactive Demonstration of How the Second Law Emerges from Interaction Networks

This project provides an intuitive, interactive demonstration of how entropy tends to increase in interacting physical systems — even in the smallest possible systems — despite the fact that the microscopic laws of motion are perfectly reversible.

The core idea:

Entropy increases when interactions destroy the special correlations present in the initial state.
Collisions create a growing interaction network.
When this network becomes connected (a percolation transition), the system loses memory of its initial configuration, and the coarse-grained entropy rises.

This project visualizes that process in real time.

---

LIVE DEMO

Run the simulation directly in your browser:

[https://galenwilkerson.github.io/index.html]

The demo shows:

• Two initially separate gas subsystems (left and right)
• Real-time particle motion and elastic collisions
• A dynamically built interaction graph (nodes = particles, edges = collisions)
• Entropy vs. time (coarse-grained, phase-space based)
• Size of the largest connected component in the interaction network
• Initial total entropy baseline (as a dashed green line)

When the partition is opened, you can watch entropy rise while the interaction network becomes connected.

---

MOTIVATION

The Second Law is often presented as mysterious or deeply tied to large numbers of particles.
But this simulation shows:

• Even two interacting particles already display entropy increase under coarse-graining.
• The increase is not due to randomness, chaos, or large-N limits.
• It comes from the destruction of correlations when energy is redistributed by interactions.
• Collisions form edges in a growing interaction network.
• When the network percolates (forms a giant connected component), the system loses memory of its initial state.
• Coarse-grained entropy rises automatically.

This connection between correlation loss, network percolation, and entropy growth removes the “mystery” from the Second Law.

---

KEY CONCEPTS ILLUSTRATED

1. Correlation destruction
   Initially, “hot” particles are on one side and “cold” particles on the other.
   After collisions, energy redistributes and the correlation evaporates.
   Entropy rises exactly because the correlation has disappeared.

2. Coarse-graining and irreversibility
   Microscopic entropy (fine-grained) is constant.
   Observed entropy increases because coarse-graining discards microscopic identity and correlation details.

3. Percolation in the interaction network
   Each collision adds an edge between two particles.
   The largest connected component grows over time.
   Once a giant connected component forms, mixing becomes global.
   Entropy rise tracks the growth of this component.

4. Minimal system demonstration
   Even a two-particle system (one hot, one cold) demonstrates:
   • mixing
   • energy exchange
   • loss of correlation
   • entropy increase under coarse-graining

This dramatically simplifies the conceptual picture of the Second Law.

---

REPOSITORY STRUCTURE

Percolation-and-Entropy/

```
index.html       Full simulation (HTML + JavaScript inline)
README.md        This overview
assets/          Optional images or screenshots
```

The entire demonstration is self-contained in a single HTML file.

---

RUNNING LOCALLY

You can run the simulation using any static server:

python3 -m http.server

Then visit:

[http://localhost:8000/index.html](http://localhost:8000/index.html)

Or simply double-click index.html.

---

RELATED PUBLISHED WORK

These are real publications that underpin the ideas of:

• entropy increase through correlation loss
• random collisions and mixing
• percolation in interaction networks
• quantum information spreading

Kac, M. (1956). “Foundations of Kinetic Theory.” Proceedings of the Third Berkeley Symposium on Mathematical Statistics and Probability.

Kac, M. (1974). “Stochasticity and Partial Differential Equations.” SIAM Review.

Bianconi, G. (2009). “Entropy of Network Ensembles.” Physical Review E, 79, 036114.

Nahum, A., Ruhman, J., Vijay, S., & Haah, J. (2017). “Quantum Entanglement Growth Under Random Unitary Dynamics.” Physical Review X, 7, 031016.

Nahum, A., Vijay, S., & Haah, J. (2018). “Operator Spreading in Random Unitary Circuits.” Physical Review X, 8, 021014.

