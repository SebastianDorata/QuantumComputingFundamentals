## 1. Ground State $|0\rangle$
$$|0\rangle = \begin{bmatrix} 1 \\ 0 \end{bmatrix} \implies \begin{aligned} P(|\psi\rangle = |0\rangle) &= |1|^2 = 1 \\ P(|\psi\rangle = |1\rangle) &= |0|^2 = 0 \end{aligned}$$

## 2. State $-|0\rangle$ (Global Phase $-1$)
$$-|0\rangle = \begin{bmatrix} -1 \\ 0 \end{bmatrix} \implies \begin{aligned} P(-|0\rangle = |0\rangle) &= |-1|^2 = 1 \\ P(-|0\rangle = |1\rangle) &= |0|^2 = 0 \end{aligned}$$

## 3. State $i|0\rangle$ (Global Phase $i$)
$$i|0\rangle = \begin{bmatrix} i \\ 0 \end{bmatrix} \implies \begin{aligned} P(i|0\rangle = |0\rangle) &= |i|^2 = 1 \\ P(i|0\rangle = |1\rangle) &= |0|^2 = 0 \end{aligned}$$

### While mathematically different, qubits measured in this state are impossible to distinguish.

---
<h1 style="text-align: center;">Global Phase</h1>

### A global phase is a complex number with a magnitude of one. 
- represented as, $e^{i\theta}$ Where $\theta$ is any real number.
$$ \boxed{e^{i\theta} = \cos\theta + i\sin\theta} $$
- When multiplying a quantum state vector $\vert\psi\rangle$
 by a global phase value, $e^{i\theta}\vert\psi\rangle$
it is physically indistinguishable from the original state.
### The global state has no observable effect on the probabilities of each outcome.

---
<h1 style="text-align: center;">Relative Phase</h1>

### A relative phase is the difference between the phase vectors of two probability amplitudes.

### Derivation: Factoring out Global Phase

**1. General Superposition State**
$$|\psi\rangle = \alpha|0\rangle + \beta|1\rangle$$

$$\Downarrow \quad \text{Rewrite coefficients in Polar Form: } z = re^{i\theta}$$

**2. Substituting Polar Coordinates**
$$|\psi\rangle = r_\alpha e^{i\theta_\alpha}|0\rangle + r_\beta e^{i\theta_\beta}|1\rangle$$

$$\Downarrow \quad \text{Factor Out } e^{i\theta_\alpha}$$

**3. Final Form with Global Phase Isolated**
$$|\psi\rangle = \underbrace{e^{i\theta_\alpha}}_{\text{Global Phase}} \left( r_\alpha|0\rangle + r_\beta e^{i(\theta_\beta - \theta_\alpha)}|1\rangle \right)$$

### Derivation: Simplifying Relative Phase

**1. Cancel Global Phase**
$$e^{-i\theta_\alpha}|\psi\rangle = \cancel{e^{i\theta_\alpha}} \left( r_\alpha|0\rangle + r_\beta e^{i(\theta_\beta - \theta_\alpha)}|1\rangle \right)$$

$$\Downarrow \quad \text{Remove Global Phase}$$

**2. Resulting State Vector**
$$|\psi\rangle = r_\alpha|0\rangle + r_\beta e^{i(\theta_\beta - \theta_\alpha)}|1\rangle$$

$$\Downarrow \quad \text{Rewrite } \theta_\beta - \theta_\alpha \text{ as just } \phi$$

**3. Final Relative Phase Form**
$$|\psi\rangle = r_\alpha|0\rangle + r_\beta e^{i\phi}|1\rangle$$


### By ignoring the global phase and simplifying the difference in phase factors to a single variable, <br> the quantum state is represented using three real numbers.
The remaining phase factor $\phi$ represents the difference in phase factors of alpha and beta.<br>
$\phi$ is something we can physically observe, and in regards to the Bloch sphere, this relative phase represents the azimuth angle around the Z axis.

--- 
