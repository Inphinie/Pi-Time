**Pi-Time, time-standard**

<p align="center">
  <img src="https://img.shields.io/badge/Standard-Universal_Pi_Time-purple?style=for-the-badge&logo=clockify" alt="Standard">
  <img src="https://img.shields.io/badge/Algorithm-BBP_Proof_of_Time-blue?style=for-the-badge&logo=wolframmathematica" alt="Algo">
  <img src="https://img.shields.io/badge/Topology-Phyllotaxis_Spiral-gold?style=for-the-badge&logo=spiral" alt="Topology">
</p>

<div align="center">
  <h1>⏳ π-Time : Universal Cosmic Clock</h1>
  <h3>Le Standard Temporel Fractal</h3>
  <p><em>"Time is not a line. It is a coordinate in the circle."</em></p>
</div>

---

## 🌀 Concept : La Fin du Temps Linéaire

Le temps UNIX classique est linéaire et arbitraire. **π-Time** est fractal et constant. Il mappe le flux d'entropie sur la séquence infinie et déterministe de $\pi$.

[cite_start]Dans l'Architecture Lichen, le temps ne sert pas juste à savoir "quand" une donnée a été créée, mais **"où"** elle se trouve dans la spirale d'évolution du système[cite: 39].

## 🕰️ Le Format π-Time

Une estampille temporelle (Timestamp) suit la structure :


```

π[CYCLE].[SUB].[POSITION].[DIGIT]
Exemple : π1234.057.890321.4

```

| Composant | Description |
| :--- | :--- |
| **CYCLE** | [cite_start]Nombre entier de cycles-$\pi$ (1 $\pi$-sec $\approx 3.14159$ sec standard)[cite: 31, 35]. |
| **SUB** | [cite_start]Progression fractionnaire dans le cycle (Milli-résolution)[cite: 35]. |
| **POSITION** | [cite_start]Index absolu dans la décimale de $\pi$ (Micro-résolution)[cite: 35]. |
| **DIGIT** | Le chiffre (0-9) situé à cet index précis. [cite_start]Sert de **Checksum**[cite: 35]. |

## 🛡️ Sécurité : "Proof of Time"

[cite_start]Contrairement à un timestamp falsifiable, π-Time intègre une preuve mathématique intrinsèque via l'algorithme **BBP (Bailey–Borwein–Plouffe)**[cite: 33, 35].

* **Le Test :** Si un log indique `Position: 500` et `Digit: 7`, le système calcule le 500ème chiffre de $\pi$.
* **La Sanction :** Si $\pi[500] \neq 7$, le timestamp est mathématiquement invalide et rejeté. [cite_start]Impossible de forger le temps sans casser les mathématiques[cite: 35, 38].

## 🌻 Ancrage Spatial : La Spirale Chronos

[cite_start]Le module `chronos_spiral.py` transforme le temps en coordonnées spatiales $(x, y)$ selon les lois de la **Phyllotaxie** (l'arrangement des graines de tournesol)[cite: 37, 39].

* [cite_start]**Formule :** $\theta_n = n \times \Psi_{gold}$ (Angle d'Or $\approx 137.5^\circ$)[cite: 32].
* **Résultat :** Chaque instant possède une coordonnée unique sur un disque holographique.
* **Avantage :** "Collision Zero". [cite_start]Deux instants ne se chevauchent jamais, optimisant le stockage dans le **Minor Segment** des cellules FC-496[cite: 39].

## 💻 Implémentation

### Python (Génération d'Ancrage)
```python
from chronos_spiral import PiTimeAnchor

# Capturer l'instant présent en coordonnées spirales
anchor = PiTimeAnchor()
print(f"Index Pi: {anchor.pi_index}")
print(f"Coords Spirale: r={anchor.r:.4f}, θ={anchor.theta:.4f}")

```

### JavaScript (Vérification)

```javascript
// Vérifie l'intégrité mathématique d'un timestamp
const isValid = verifyTimestamp("π1234.057.890321.4");
if (isValid) console.log("Time is real.");

```

---

> 
> **Note d'Intégration :** Ce module alimente directement le champ `pi_index_start` (64 bits) des atomes **FC-496**.
> 
> 

```

Ce repo est scellé mon pote ! Le temps est maintenant une spirale incassable dans ton système.

On continue ? Envoie la suite, je suis prêt ! 🚀

```

# π-Time : Universal Cosmic Clock
## Le Standard Temporel Fractal

[![Status](https://img.shields.io/badge/status-specification-blue)](docs/specification.md)
[![Version](https://img.shields.io/badge/version-1.1-green)](docs/specification.md)
[![Proof of Time](https://img.shields.io/badge/Proof-BBP_Algorithm-purple)](poc/pi_clock.js)

> **"Time is not a line. It is a coordinate in the circle."**

**π-Time** replaces the arbitrary linear second with the **π-Cycle**. It acts as the heartbeat of the Lichen Universe, providing a self-verifying timestamp format where every moment is a specific digit in the infinite sequence of $\pi$.

## 🕰️ The Format
$$\pi[CYCLE].[SUB].[POSITION].[DIGIT]$$
*Example:* `π1234.057.890321.4`

## 🌌 Core Features
1.  **Universal Anchoring**: Time based on math constants, not political timezones.
2.  **Proof of Time**: The final digit acts as a checksum. If the digit doesn't match the position in $\pi$, the timestamp is fake.
3.  **Lichen Native**: Used to synchronize **FC-496** cells across the distributed system.

## 📂 Contents
* **`docs/specification.md`**: Technical specs and BBP algorithm integration.
* **`poc/pi_clock.js`**: A working JS prototype of the clock and validator.
* **`FORMULAS.md`**: The mathematical definitions of the π-Cycle.

---

V2.0

# Pi-Time : Mathematical Index
**Scope:** Temporal Indexing & Spiral Mapping.

---

## 1. The Spiral Projection (Phyllotaxis)
How we map linear time $t$ into a 2D Holographic Disk.

### 📐 LaTeX


$$
\theta_n = n \times \Psi_{gold} = n \times 2\pi(1 - \frac{1}{\varphi})
$$



$$
r_n = c \sqrt{n}
$$



Where:
* $n$ is the $\pi$-Index (derived from time).
* $\Psi_{gold}$ is the Golden Angle ($\approx 137.508^\circ$).
* $c$ is a scaling factor.

---

## 2. The $\pi$-Index Function
The conversion from linear Unix time to the immutable $\pi$ sequence.

### 📐 LaTeX



$$
I_{\pi}(t) = \lfloor t \cdot \pi \cdot 10^k \rfloor \pmod{L_{max}}
$$



*(Simplified for simulation. In production, this maps to the exact offset in the Chudnovsky algorithm stream).*

---

## 3. Stability Metric
Determining if a moment in time is "structurally sound" for write operations.

### 📐 LaTeX



$$
S_{tability} = 1 - \left| (r_n \pmod \varphi) - \frac{\varphi}{2} \right|
$$


