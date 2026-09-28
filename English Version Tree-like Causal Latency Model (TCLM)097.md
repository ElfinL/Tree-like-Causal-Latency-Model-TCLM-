# Tree-like Causal Latency Model (TCLM) and Dual-Pulse Synchronization Protocol (DPSP): From Observational-Delay Deconstruction to Interplanetary and Cross-Galactic Deep-Space Chronometric Engineering

> **Language Disclaimer**
> In the event of any discrepancy or inconsistency between this English version and the original Chinese version, the Chinese version shall prevail.

**Author**: Lee Wang Hin (李泓軒, Elfin)  
**Affiliation**: Independent Researcher  
**Publication Date**: September 2026

> **Manifesto**
> Newton was right, and Einstein was also right.  
> The causal tree is a framework that allows both to be true simultaneously.

---

## Abstract

This paper focuses on two main points. First, it points out that directly equating the mathematical boundary failure of the Lorentz transformation at $v > c$ with "time flowing backward" misplaces the propagation latency of observation signals as a reversal of physical time. Second, it proposes the Dual-Pulse Synchronization Protocol (DPSP), which uses ex-post comparison of timestamps from optical events and entangled events to separate spatial latency from the local time-flow rate. The remaining chapters cover engineering calibration, extended applications, and boundary defenses. The objective of this paper is to establish a framework for spacetime causal-reconstruction theory and its accompanying deep-space timekeeping engineering.

To this end, the "Tree-like Causal Latency Model (TCLM)" is proposed, which strictly decouples time into a "Topological Causal Order (Topological Trunk)" and a "Geometric Time-Rate Difference (Geometric Branches)." The topological trunk ($\mathcal{C}_{\text{trunk}}$) is not a Newtonian global absolute clock, but a strictly one-way topological causal-order index ($\operatorname{sgn}(\mathcal{C}) \equiv +1$) describing the underlying event settlement of the universe. The geometric branches represent the proper-time rate and geometric observation latency of local physical entities under specific gravitational potential and velocity fields.

To advance this theory into engineering practice, this paper also proposes a top-level communication standard: the "Dual-Pulse Synchronization Protocol (DPSP)." This protocol breaks the traditional master-slave time-synchronization paradigm that treats a specific celestial body (such as Earth) as a privileged reference frame, establishing a **Decentralized Initial-Constant Locking and Local Rate Measurement** mechanism. All nodes (whether on Earth, Mars, or deep-space vehicles) act as equal branch observers, decoupling the "local time-rate factor ($\Gamma$)" and the "initial integration constant ($t_0$)" at a dual-logical level.

- At the local end, at least two sets of independent pulse units of different lengths are established.
- Each set contains a local atomic-clock timestamp of a quantum-entanglement local measurement event (recorded locally; pairing requires classical ex-post comparison) and a classical electromagnetic return pulse.
- Through multi-baseline cross-correlation and spacetime-vector triangulation, the local branch curvature is single-point solved.
- At the deep-space end, only a very low-frequency (or single) initial handshake pulse is required to lock the initial integration constant $t_0$.

To address the dynamically and continuously fluctuating time field, the protocol further introduces "Adaptive Pulse Frequency Scaling," "Continuous Curvature Quadratic Compensation," and "Causal Backpressure Buffer" mechanisms. Through continuous field integration along the spacetime worldline (Worldline Path Integration), the causal order relative to the initial handshake ($\mathcal{C}_{\text{trunk}} - t_0$) is independently reconstructed in dynamic gravity wells and non-inertial frames. This achieves an engineering leap from "interplanetary relative calibration" to "causal-order reconstruction relative to the initial handshake." In principle, the architecture can be extended to interstellar and even cross-galactic scales. This paper uses the Earth–Mars system as the first-stage engineering calibration case; engineering feasibility and error budgets at cross-galactic scales remain topics for future research.

Combining surface GPS (+38 μs/day) and Earth–Mars system (477 μs/day) astronomical data as input calibration cases for relativistic time rates supports the theoretical feasibility of this protocol under multi-frequency dispersion compensation and given mission-geometry assumptions. The theoretical resolution of local time-flow-rate measurement is constrained by the hardware limits of current optical lattice clocks (in terms of fractional frequency stability, currently reaching the $10^{-18}$ to $10^{-19}$ order of magnitude). In the Earth–Mars case, after multi-frequency dispersion compensation and ephemeris constraints, the engineering alignment error-budget target is at the nanosecond level ($\mathcal{O}(10^{-9}\text{ s})$). A significant gap remains between this target and the precision actually achievable by current deep-space links, mainly limited by plasma residuals, ephemeris uncertainties, and signal-to-noise ratios, pending end-to-end link simulation and empirical validation. This paper does not claim that the architecture already possesses gravitational-wave detection capabilities.

---

## Introduction and Epistemological Disclaimer

This theory employs information-theoretic physics and topological geometry for the structural description of causal chains in physical spacetime. The abstract concepts used in this paper, such as "static topological full map," "restricted read order," and "information propagation latency," are strictly confined to the domain of information theory and mathematical models, aiming to provide an objective deconstruction of physical observations without making any metaphysical assumptions or extensions regarding the ontological entity of the universe.

---

## Chapter 1: From "Faster-than-Light Time Travel" to the Distinction Between Causal Order and Time

The core intuition of this paper can be illustrated by thunder and lightning.

The existence of thunder and the lightning we observe are two different things.

If we perceive the existence of thunder in some way before the lightning arrives, does that mean we have traveled back in time?

No. It simply means that the latency of our perception method is shorter than that of the lightning. The event itself has not reversed; only the signal latency has been shortened.

Because there is only one thunder event, it occurred. But it takes time for the lightning to travel from the location of the thunder to our location. Therefore, the lightning we see was emitted by the thunder at a past moment. What we see is always the past lightning, not the thunder itself.

If we treat the "order of seeing the lightning" as the "order of the thunder occurring," we would falsely assume the occurrences have a sequence. But if we clearly distinguish between the "existence of the thunder itself" and the "arrival time of the lightning," we realize: there is only one thunder; only the arrival times of the lightning differ.

This distinction is the first cornerstone of TCLM. This paper will formally define this distinction in Chapter 2. Let us first start with a more fundamental question to explain why this distinction is important.

**Are "the order of observation" and "the order of occurrence" the same thing?**

If they are not the same thing, then the claim of "faster-than-light going back in time" needs to be re-examined. The result of this examination is: going back in time faster than light seems possible only because "observation latency" and "event occurrence" are conflated. The Lorentz transformation yields imaginary numbers when $v > c$. The standard formulation in physics textbooks is "no real solution, hence unreachable for particles with mass." If this complex output is directly interpreted as "time flowing backward," it confuses two concepts.

But this misinterpretation happens to open a door: if causal order and time are not the same thing, then what are they respectively? What is their relationship?

This is the starting point of the Tree-like Causal Latency Model (TCLM). Below, we will first explain the mathematical boundary failure of the Lorentz transformation at extreme speeds, and then explain how this boundary leads to the distinction between causal order and time.

### 1. The Mathematical Boundary Failure of the Lorentz Transformation at Extreme Speeds

Traditional special relativity faces two core mathematical collapses when dealing with extreme speeds, both rooted in "forcing the electromagnetic propagation limit ($c$) to be equivalent to the ontological time of the universe":

1. **Observed Time ($t'$) Exceeding the Real Domain**:
   In the transformation equation $t' = \frac{t - \frac{v x}{c^2}}{\sqrt{1 - \frac{v^2}{c^2}}}$, when $v > c$, the denominator $\sqrt{1 - \frac{v^2}{c^2}}$ becomes imaginary, pushing the entire $t'$ into the complex domain. Whether the numerator is negative depends on specific values. If this complex output is directly interpreted as "time flowing backward," it is fundamentally a misjudgment of invalid values given by the formula beyond its real domain as an actual reversal of physical time.

2. **Proper Time ($\tau$) Exceeding the Real Domain**:
   In the proper-time formula $\tau = t \sqrt{1 - \frac{v^2}{c^2}}$, when $v > c$, an imaginary number $i$ is calculated. This is the mathematical model exceeding its real domain (undefined over the real domain), not the physical structure of time turning into nothingness.

### 2. The Fundamental Nature of the Boundary Failure

The Lorentz transformation yields imaginary (complex) values when $v > c$. If this complex output is directly interpreted as "time flowing backward," two concepts are confused:

- **Mathematical Model Failure**: The input of the formula exceeds its valid range, thus yielding an invalid output.
- **Physical Impossibility**: Natural laws prohibit the existence of this phenomenon based on first principles.

This paper merely points out that the Lorentz transformation exceeds its applicable domain when $v > c$, and does not directly infer that faster-than-light (FTL) is necessarily viable. If FTL exists, it still requires an independent causal-propagation theory to support it.

### 3. From Boundary Failure to the Distinction Between Causal Order and Time

This mathematical boundary failure leads to a more fundamental distinction:

**The order in which events occur (causal order) and the order in which an observer receives signals (observed time) are not the same thing.**

"Faster-than-light going back in time" appears possible precisely because these two are conflated. If they are separated, FTL no longer implies going back in time, but simply a reorganization of observation latency.

This distinction is the first cornerstone of TCLM.

**Scope of this Paper**

This paper does not conduct a systematic literature review. Existing concepts mentioned herein are solely used to illustrate the boundaries of this paper's framework and do not constitute a complete citation or evaluation of related literature. This paper does not claim to have pioneered the concept of "quantum-entanglement timestamps." Based on the common premise that the latency of entanglement correlations is far below currently measurable precision, this paper treats entanglement events as a candidate source of local timestamps and derives the DPSP engineering framework accordingly; this paper does not claim to have verified its practicality, nor does it claim to have pioneered the concept.

---

## Chapter 2: Core Postulates and Global Causal Equation of the Tree-like Causal Latency Model (TCLM)

### 1. Core Postulates

To repair the mathematical collapse of relativity under extreme conditions, we establish the following postulates, strictly decoupling the "topological causal order (trunk)" of the physical world from the "relative observation latency (branches)":

* **Postulate 1: Topological Causal Order and Geometric Branch Curvature**

  * **Topological Causal Trunk ($\mathcal{C}_{\text{trunk}}$)**: It is a mathematical index (topological sort) of the strictly one-way causal sequence between events. It is not a directly measurable physical clock itself, nor does it presuppose any observable privileged simultaneity slice. Whenever $\mathcal{C}_{\text{trunk}}$ appears in the formulas of this paper, it refers to the second-parameterized version defined by the affine transformation $\mathcal{C}_{\text{trunk}} \mapsto a\mathcal{C}_{\text{trunk}} + b$ under initial-handshake reference normalization, with seconds as the unit. Its absolute zero point has no physical meaning; only the difference $\Delta \mathcal{C}_{\text{trunk}}$ is meaningful. This normalization does not affect the chronological order of events, but guarantees the uniqueness of differences, integrals, and $t_0$.

  Time (proper time) is inherently a local concept. Since the time-flow rate of different systems fluctuates continuously with gravitational potential and motion state, there is no "time" reading that can be directly shared across systems. Observers cannot directly see each other's time; they can only reconstruct the causal sequence between events ex-post via signal latencies and local clock records. Thus, the role of $\mathcal{C}_{\text{trunk}}$ in this framework is this consistently reconstructable causal-order index.

  Analogy: The position of the sun in the sky is not time itself; it is a physical state. A sundial maps this physical state into a time reading. Similarly, $\mathcal{C}_{\text{trunk}}$ itself is not time; it is a causal order. $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$ is the function mapping this causal order to the branch proper time. What we can actually reconstruct is the integral quantity relative to the initial handshake constant $t_0$.

  * **Geometric Relative Branches and Curvature**: Represents the relative observation trajectories and local proper-time rates ($\tau$) of physical entities growing out of the causal trunk. The essence of relative time-flow rates is the curvature of the branches on a four-dimensional geometric manifold. Relativistic effects measured by local observers (e.g., time dilation, gravitational redshift) are all results of path integrals on the geometric branches.

  * **Dynamic Environmental Adaptability (Continuous Curvature-Field Fluctuation)**: Physical entities are not locked into the hierarchical structure of specific celestial bodies. Spacetime curvature is intrinsically a continuously floating field, fluctuating dynamically with the current gravitational potential and velocity field. When an object moves across galaxies, its ontological branch directly adapts to the local continuous geometric curvature. Between all objects, there only exists a "relative time difference induced by current geometric curvature," while they mutually share the exact same global causal order.

  * **Forward Growth Constraint**: Under the causal-direction constraint ($\operatorname{sgn}(\mathcal{C}) \equiv +1$), the growth vectors of all branches are strictly one-way downstream. The causal direction is always positive and absolutely prohibits reverse growth back upstream to the trunk within a single manifold.

  **Epistemological Note on "Now" and the Sense of Simultaneity**

  The subjective feeling of "now" and "being in the same moment as the other party" is the result of the local nervous system integrating short-latency signals, not a globally given physical simultaneity. All perceived information carries a propagation latency and is intrinsically a reconstruction of the past. At everyday scales, where light latency is extremely short and relative speeds are very low, this approximation is valid; once the distance increases or relative motion becomes significant, the approximation fails. What can be objectively shared physically and reconstructed consistently is solely the causal sequence of events.

* **Postulate 2: Decoupling of Event Ontology and Signal Carrier (The Isomorphic Model of Thunder and Lightning)**

  * **Decoupling of the Event Ontology and Lightning**: Using the "existence of the thunder/lightning event ontology" and "the lightning propagating outward" as an isomorphic model: the instant a thunder event is settled on the topological trunk ($\mathcal{C}_{\text{trunk}}$) is the settlement point of that physical entity in the topological causal order. The lightning received by the observer is merely the geometric branch signal propagating outward from that event ($t_{\text{observed}} = \tau_{\text{branch}}(\mathcal{C}_{\text{trunk}}) + \Delta t_{\text{latency}}$).

  * **Limit of Propagation vs. Time Ontology**: Lightning is only a carrier for transmitting information (geometric branch); its propagation latency does not equal the occurrence time of the thunder event itself. Even if one commands a propagation method exceeding the speed of light (perceiving the thunder event faster than lightning), it merely means the signal-transmission latency has been shortened (flattening the branch); it absolutely does not mean the observer has traveled back before the thunder event occurred (causal settlement).

### 2. Global Causal Equation and Dual-Layer Geometric Decoupling

The TCLM global causal equation adopts a dual-layer modular architecture, decoupling macroscopic topological causality from the microscopic geometric-field latency mechanism:

$$t_{\text{observed}} = \tau_{\text{branch}}(\mathcal{C}_{\text{trunk}}) + \Delta t_{\text{latency}}$$

Where $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$ is the proper time on the branch where the event is located, corresponding to the causal order $\mathcal{C}_{\text{trunk}}$. It is a mapping from "causal order $\rightarrow$ time reading." It does not depend on the observer; what the observer depends on is $\Delta t_{\text{latency}}$.

Note here: $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$ and $t_{\text{observed}}$ may belong to different worldlines. Their addition is a formal combination mapped under the same causal-order index after being parameterized by a common causal order; it is not the direct arithmetic sum of the proper times of any two arbitrary worldlines.

**Operational Definition:** In the equation above, $\mathcal{C}_{\text{trunk}}$ is an inaccessible quantity; what DPSP actually measures locally is the "interval ratio of the same set of events on two clocks":

$$\Gamma_{\text{local}}(\tau) \equiv \frac{\Delta \tau_{\text{local}}}{\Delta \tau_{\text{base}}}$$

Where $\Delta \tau_{\text{local}}$ is the interval measured by the local clock between two events, and $\Delta \tau_{\text{base}}$ is the interval measured by the base clock between the same two events. This ratio is directly measurable and can be greater than, equal to, or less than 1. $\mathcal{C}_{\text{trunk}}$ is a post-calculated reconstructed integral quantity; its full form is in Chapter 3, Section 2.

*(Note: This formula accounts for the spatial geometric-latency part; the complete time rate must incorporate gravitational redshift, detailed in Chapter 4 calibration.)*

The microscopic geometric-field latency quantity is defined as:

$$\Delta t_{\text{latency}} \equiv \int_{\mathcal{P}} \frac{\sqrt{g_{ij}^{\text{branch}} dx^i dx^j}}{v_{\text{signal}}(x)}$$

(The causal-order parameter $\mathcal{C}_{\text{trunk}}$ satisfies strict monotonic increment; the integral term is comprehensively determined by geometric distance, propagation speed, and branch curvature, and is always positive, measured in seconds. In engineering implementation, this geometric latency is mapped locally as the difference between classical optical timestamps and entangled-event timestamps; see Chapter 3, Section 1.3.)

**Parameter Symbol Explanations**:

* $t_{\text{observed}}$: The scalar time when the observer receives the information residue in a specific coordinate system.
* $\mathcal{C}_{\text{trunk}}$: The underlying causal-settlement scalar of the event's occurrence, satisfying the strict monotonic-increment postulate (monotonically increasing along the proper time $\tau$ of any physical worldline, i.e., $\frac{d\mathcal{C}_{\text{trunk}}}{d\tau} > 0$). It represents the topological causal position of the event, not a globally synchronized physical clock.
* $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$: The proper time on the branch corresponding to the causal order $\mathcal{C}_{\text{trunk}}$.
* $\Delta t_{\text{latency}}$: The geometric latency accumulated by information propagating in the branch-space manifold, in seconds (s), strictly positive ($\Delta t_{\text{latency}} \ge 0$). This is a geometric definition; its operational definition is the local clock difference $\Delta\tau_{\text{local}} = t_{\text{light}} - t_{\text{entanglement}}$, see Chapter 3, Section 1.3.
* $\mathcal{P}$: The physical geometric path traversed by the information carrier in the 3D branch-space manifold.
* $g_{ij}^{\text{branch}}$: The positive-definite geometric tensor describing local spatial curvature, gravitational potential, and information-propagation limit resistance ($i, j \in \{1, 2, 3\}$).
* $dx^i, dx^j$: The infinitesimal coordinate displacement of the information carrier advancing along the spatial propagation path.
* $v_{\text{signal}}(x)$: The effective propagation rate of the information carrier at coordinate point $x$ (e.g., effective light speed of EM waves in a local field, satisfying $v_{\text{signal}}(x) > 0$), ensuring the formula possesses rigorous time dimensions $[\text{m}] / [\text{m/s}] = [\text{s}]$.

All references to "causal-order reconstruction" in this paper refer to this second-parameterized quantity.

**Intuitive Understanding: The Inaccessibility of $\mathcal{C}_{\text{trunk}}$**

Both $\mathcal{C}_{\text{trunk}}$ and $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$ are directly inaccessible. $\mathcal{C}_{\text{trunk}}$ can be likened to the order represented by a still water surface, while $\tau_{\text{branch}}$ is the proper time mapped from that water surface onto the observer's branch. However, the observer can never directly touch the still water surface:

- The water itself is a continuous fluctuating field (dynamic $\Gamma_{\text{local}}(t)$); it is always flowing.
- The act of measuring, like touching water with a ruler, inevitably causes ripples (introducing $\Delta t_{\text{latency}}$).

Therefore, what the observer can touch is always "flowing water surface + ripples" ($t_{\text{observed}}$), not the still water surface itself. $\mathcal{C}_{\text{trunk}}$ is the order represented by this limit; it exists independently of the water and ripples but cannot be directly touched.

Although inaccessible, it can be indirectly reconstructed via the "interval ratio":

From the operational definition above, $\Gamma_{\text{local}}$ is the interval ratio directly measured locally by DPSP.

$\mathcal{C}_{\text{trunk}}$ is the post-calculated reconstructed integral:

$$\mathcal{C}_{\text{trunk\_reconstructed}}(\tau) = t_0 + \int_{\tau_0}^{\tau} \Gamma_{\text{local}}(\tau')\, d\tau'$$

**The sequence is: measure the interval ratio first, then integrate to reconstruct the causal order.** It is not defining a causal order first and then calculating the interval ratio. This assumes the initial-handshake reference is normalized to $\Gamma_{\text{trunk,base}}=1$; if the reference is not curvature-free, the full form must include the $\Gamma_{\text{trunk,base}}$ factor, see Chapter 3, Section 2.

If using the geometric-projection definition $\Gamma_{\text{trunk}}=\sec\theta\ge 1$, then $d(\mathcal{C}_{\text{trunk}}-t_0)/d\tau=\Gamma_{\text{trunk}}$.

**Premise:** This reconstruction involves the inherent latency of a second set of local events (currently envisioned as quantum-entanglement events). This latency is not a necessary condition for the reconstruction to be valid; if it is zero, $\mathcal{C}_{\text{trunk\_reconstructed}}$ directly corresponds to $\mathcal{C}_{\text{trunk}}$; if it is a tiny non-zero value, there exists an unknown constant offset between $\mathcal{C}_{\text{trunk\_reconstructed}}$ and $\mathcal{C}_{\text{trunk}}$, which only affects the absolute value but not the chronological order. Under current optical-lattice-clock precision, this latency is indistinguishable. The core condition for DPSP is not whether this latency is zero, but whether it is affected by different factors than optical latency, whether it is stable enough, and whether it is significantly smaller than optical latency; see Chapter 3, Section 1.2.

**Analogy: The Sundial and $\tau_{\text{branch}}$**

The sun's position is not time itself; it is a physical state. A sundial maps this to a time reading. Similarly, $\mathcal{C}_{\text{trunk}}$ is a causal order, and $\tau_{\text{branch}}$ maps this order to a proper time on the branch. Both can be calculated indirectly, differing only in the length of the reconstruction chain.

**Symbol Conventions (Unified Throughout):**

* $\Gamma_{\text{trunk}}$: Local geometric dilation factor relative to the ideal curvature-free trunk limit, $\Gamma_{\text{trunk}} = \sec\theta \ge 1$.
* $\Gamma_{\text{local}}$: Operational measurement ratio locally relative to the initial handshake reference, $\Gamma_{\text{local}} = \Delta\tau_{\text{local}} / \Delta\tau_{\text{base}}$. May be greater than, equal to, or less than 1.
* $\gamma_{B/A}$: Relative time-rate variation between two endpoints, $\gamma_{B/A} = d\tau_B / d\tau_A$.
* $\lambda(t)$: Target flow-rate ratio relative to the source, $\lambda(t) = d\tau_{\text{target}} / d\tau_{\text{source}}$, used for adaptive pacing.

These four must not be conflated.

This protocol directly measures the interval ratio $\Gamma_{\text{local}}$; the causal order $\mathcal{C}_{\text{trunk}}$ is a post-calculated integral quantity. The two must not be conflated.

### 3. Historical Confusion of Absolute and Relative Time: TCLM's Decoupling Perspective

In physics history, Newtonian absolute time and Einsteinian relative time have long been viewed as incompatible.

Newtonian absolute time presupposes:

> A universal time background flowing uniformly, independent of matter, shared across the entire universe.

Einsteinian relative time points out:

> Time is not an independent background; it and space together constitute a geometric manifold. Under different gravitational potentials and motion states, time-flow rates inherently differ.

If the two are treated as mutually exclusive answers to the same question, conflict is inevitable.

However, TCLM points out that this conflict arises from conflating two different dimensions of description into one.

What Newton truly wanted to guarantee was not "identical time," but "irreversible causal order."  
What Einstein truly described was not "reversible causality," but "local time flow varying with geometry."

In TCLM:

- Newton's absolute time → corresponds to the global causal order $\mathcal{C}_{\text{trunk}}$ and its mapping requirement $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$.
- Einstein's relative time → corresponds to the geometric branch latency $\Delta t_{\text{latency}}$.

They do not contradict, because they answer fundamentally different questions.

What Newton saw was the trunk of the tree; what Einstein saw was the branches.  
They merely stood before the same tree, pointing out different dimensions.

Therefore, TCLM does not advocate returning to Newton, nor does it deny Einstein.  
It merely places "causality" and "time" — which have been conflated — back into their respective positions.

**Why the Lorentz Transformation's $t=0$ Is Not Absolute:**

The Lorentz transformation is correct when $v < c$. But its $t=0$ relies on the Einstein synchronization convention, which is based on the speed of light. Different observers using light to synchronize clocks obtain different simultaneity slices, so $t=0$ is not absolute. TCLM does not deny this result; TCLM merely points out that the non-absoluteness of $t=0$ is a property of geometric projection and does not conflict with the absoluteness of the underlying causal order $\mathcal{C}_{\text{trunk}}$.

---

## Chapter 3: Deep-Space Engineering Implementation: Dual-Pulse Synchronization Protocol (DPSP) and Initial-Handshake Causal-Order Reconstruction

**Symbol Note**: This chapter follows the "Symbol Conventions (Unified Throughout)" of Chapter 2. Unless otherwise subscripted, $\Gamma$ refers to $\Gamma_{\text{local}}$. $\Gamma_{\text{trunk}}$, $\Gamma_{\text{local}}$, $\gamma_{B/A}$, and $\lambda(t)$ must not be conflated.

### 0. Operational Core

This section first explains the core operational principle of DPSP, before entering into terminology and formulas.

**Core Principle: Measuring local clock interval ratios, rather than absolute time readings.**

The specific operations are as follows:

1. The central node emits classical optical pulses at fixed local-clock intervals while simultaneously triggering quantum-entanglement events. The central node records its own emission timestamps and local entanglement-event timestamps.
2. The receiving ends record the local arrival timestamps of both the classical light and the entangled events upon receipt.
3. The receiving ends transmit these two timestamps back to the central node via a return channel. The return-channel timestamp is not included in the computation.
4. The central node uniformly receives the timestamps from all receiving ends, compares them with its own recorded emission and entanglement-event timestamps, and computes the interval ratio $\Gamma_{\text{local}}$.

This operation has three important properties:

- **No prior clock synchronization between the two ends is needed.** The absolute readings of the emitter and receiver are irrelevant; what matters is the interval ratio.
- **The fluctuation of the emitter's clock is itself the signal.** If the emitter's clock runs fast, the emission interval shortens; if slow, it lengthens. This variation is directly reflected in the arrival interval measured at the receiving end. We do not need to know how fast the emitter "should" run — only how much it "actually" ran.
- **The only error source to handle is the variation of the optical propagation path.** If the optical path changes between two measurements, the measured interval at the receiving end will simultaneously contain both the clock-rate difference and the optical-latency variation. The multi-baseline design is intended to separate these two.

**Role of Multiple Baselines:**

If the optical path is stable, a single baseline suffices. Multiple baselines are not for clock synchronization but for separating, when the optical path changes, "the geometric-latency variation proportional to baseline length" from "the clock-rate difference independent of baseline length."

**Role of Quantum-Entanglement Event Timestamps:**

It is the second set of local event timestamps, used to provide a local reference independent of the classical optical path. It is not a necessary condition for this protocol, nor is it the most central part. The core operation is always: the emitter emits at fixed local intervals; the central node computes the interval ratio.

**Difference from Traditional Architectures:**

Traditional deep-space timekeeping requires high-frequency bidirectional handshakes because it attempts to align the clock readings of both ends. DPSP does not require reading alignment — only the interval ratio. The initial handshake locks only one integration constant $t_0$, not clock readings.

The following sections are the engineering formalization, precision refinement, and error handling of this operational core.

#### 0.1 Engineering Motivation & Necessity

Traditional deep-space timekeeping architectures assume the time-flow rate to be a predictable constant or static offset. Under the TCLM framework, however, the local time-flow-rate factor relative to the initial handshake ($\Gamma_{\text{local}}$) is intrinsically a continuously floating field affected by gravitational and velocity fields. This property gives rise to three major deep-space timekeeping bottlenecks, which also constitute the engineering necessity for this protocol:

1. **Local Imperceptibility**:
   When a single observation node is located on a fixed celestial body (e.g., Earth's surface), the local curvature-gradient variation is extremely small, so the time-flow-rate fluctuation is virtually imperceptible in short-term measurements. Observers easily mistake the time-flow rate for a constant, thereby overlooking the dynamic corrections needed for alignment relative to the initial handshake.

2. **Interplanetary Scale Amplification**:
   Once the endpoint crosses to deep space (e.g., the Earth–Mars system), the tiny differences in local curvature and potential are continuously accumulated and amplified through time integration. The Earth–Mars time-flow-rate difference can reach the $477\,\mu\text{s/day}$ order (with a $\pm 226\,\mu\text{s/day}$ variation depending on orbital position), and this difference varies dynamically with orbital eccentricity, solar gravitational-potential perturbations, and celestial perturbations, making long-term extrapolation with a single fixed constant impossible.

3. **Infeasibility of Continuous Sync**:
   If one attempts to rely on high-frequency bidirectional signals for continuous phase-locking, two limits arise: first, the **light-speed propagation-latency limit** (e.g., Earth–Mars one-way delay of 3 to 22 minutes, making real-time feedback impossible); second, the **unpredictability of continuous dynamic perturbations**, which causes any fixed mathematical extrapolation to diverge over time.

#### 0.1.1 Applicability Boundary

DPSP is not intended to replace all deep-space timekeeping architectures, nor is it necessary in all scenarios. Its applicable conditions are:

1. **Sufficient local compute**: The node must be capable of cross-correlation, geometric reconstruction, and continuous integration. If local compute is insufficient, traditional telemetry-based timekeeping suffices.
2. **Tolerance of communication blackouts**: If the mission permits continuous high-frequency handshakes and the link is stable, traditional DSN timekeeping already meets requirements. The primary value of this protocol lies in providing offline autonomous timekeeping capability.
3. **Interplanetary or longer-term missions**: For near-Earth or short-term missions, the relative time-flow-rate difference is extremely small, and the engineering benefit of introducing this protocol is limited.

In short, DPSP is an offline time-reconstruction solution designed for "long-term, offline, high-compute" deep-space nodes, not a universally required solution.

#### 0.2 Paradigm Shift: From "Earth-Model Dependency" to "Local Physical Measurement"

The fundamental limitation of traditional deep-space timekeeping (e.g., Deep Space Network) lies not only in the master-slave ideology of treating Earth as a privileged reference frame, but also in its methodological dependence on Earth-side astronomical formulas and ephemeris models. A deep-space node lacks the capacity to measure its own time-flow rate and can only passively receive calibration parameters computed on Earth. Once communication is interrupted or the ephemeris model becomes invalid, the node loses temporal autonomy.

Under the TCLM framework, Earth time ($t_{\text{Earth}}$) and Mars time ($t_{\text{Mars}}$) are both merely "geometric branch residues" under local gravity wells and motion states; neither is an objective time reference of the universe.

The fundamental breakthrough of DPSP lies in granting any deep-space node the ability to perform "local physical measurement." The node no longer needs to query Earth's gravitational-field formulas; it directly measures its own time-flow-rate variation relative to the initial handshake ($\Gamma_{\text{local}}$) via local event interval-ratio measurement. Earth-computed models serve only as initial references, not as the sole source of truth.

| Conceptual Dimension | Traditional Deep-Space Timekeeping (DSN-type) | Dual-Pulse Synchronization Protocol (DPSP / TCLM Topological) |
| :--- | :--- | :--- |
| **Reference-frame positioning** | Earth-privileged reference frame (Master-Slave) | Decentralized, no-privileged node (Decentralized Nodes) |
| **Alignment target** | Follow Earth time $t_{\text{Earth}}$ | Directly measure time-flow-rate variation relative to the initial handshake ($\Gamma_{\text{local}}$) |
| **Communication dependency** | High-frequency/continuous bidirectional handshake to maintain phase lock | Only initial-value lock; thereafter, local differential autonomous computation |
| **Physical essence** | Engineering compromise to compensate for signal delay | Observer's decoding of the universe's underlying topological causal order |

Based on the above paradigm shift, this protocol abandons the traditional high-frequency bidirectional phase-locking architecture, decoupling the "local time-flow-rate factor ($\Gamma_{\text{local}}$)" and the "global initial constant ($t_0$)" at a dual-logical level, and establishing a multi-layer dynamic control system. This mechanism may be termed **Decentralized Initial-Constant Locking and Local Rate Measurement**.

This paper uses the Earth–Mars system as the first-stage engineering calibration case. The applicability of DPSP is not limited to interplanetary distances; provided an initial handshake can be completed, the subsequent autonomous reconstruction and communication-blackout tolerance can, in principle, be extended to interstellar and even intergalactic scales.

**DPSP's Output Is Causal Order; Time Is Derived from Causal Order.**

It should be particularly emphasized: the objective of this protocol is not to align the clock readings of the two ends, nor to directly measure "time." Under the TCLM framework, the causal order $\mathcal{C}_{\text{trunk}}$ is fundamental, and the time reading $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$ is a product mapped from the causal order. This relationship is like the sundial: the sun's position in the sky is not time itself; the sundial maps this physical state into a time reading. Similarly, the causal order is not time; $\tau_{\text{branch}}$ maps the causal order to the branch proper time.

What DPSP reconstructs is the causal order relative to the initial handshake:

$$\mathcal{C}_{\text{trunk\_reconstructed}}(\tau) = t_0 + \int_{\tau_0}^{\tau} \Gamma_{\text{local}}(\tau')\, d\tau'$$

Once the causal order is reconstructed, the local time reading can be obtained by mapping $\tau_{\text{branch}}(\mathcal{C}_{\text{trunk}})$. The absolute-reading offset between the two clocks naturally cancels in this process and does not affect the reconstruction of the causal order. What the initial handshake locks is the integration constant $t_0$, not clock alignment.

---

### 1. Layer 1: Local Spacetime-Vector Triangulation

**Node Hardware Configuration**

The basic node configuration comprises: (1) a local atomic clock; (2) a quantum-entanglement source; (3) at least two optical baselines of different lengths, each with classical optical transceiver modules at its endpoints; (4) a multi-baseline cross-correlation processing unit. The starting points of the two baselines must coincide, so that the delay difference arises solely from the baseline-length difference.

**Definition of Dual-Pulse**

The "dual-pulse" referred to in this protocol means that at least two sets of baselines of different lengths are established at the local end, with two independent pulse units triggered simultaneously.

Each pulse unit contains a local timestamp of a quantum-entanglement measurement event and a local timestamp of a classical electromagnetic return pulse.

A single baseline provides only a one-dimensional projection of the delay difference and cannot uniquely solve for the geometric deflection angle of the spacetime manifold.

Therefore, the minimum requirement of the dual-pulse is two baselines of different lengths; if a third baseline of different length is available, a closure method can further verify the uniqueness and measurement stability of the $\theta$ solution.

**Internal Operation of a Single Pulse Unit (Quantum-Classical Coupled Measurement)**

For any independent baseline (endpoints $L_1, L_2$), the single pulse measurement contains two inseparable physical steps, strictly obeying the quantum no-communication theorem:

- **Step 1: Local Timestamp of the Quantum-Entanglement Measurement Event**:
  Using a locally pre-entangled quantum system, measurements are independently triggered at both ends $L_1$ and $L_2$. The single-sided reduced density matrix ($\rho = \frac{1}{2}I$) exhibits only random statistical eigenvalues and cannot transmit real-time information. However, each measurement is a local event, and the local atomic clock records its event timestamp. This timestamp does not change with the classical propagation-path delay; it is compared ex-post with the classical optical return timestamp.

- **Step 2: Classical Latency Return**:
  Along the same baseline, the opposite end ($L_2$) encodes the ex-post-read measured data stream (including the quantum-entanglement event timestamp and the classical optical return timestamp) as a classical electromagnetic signal and transmits it back to the local end ($L_1$). Its propagation trajectory constitutes a standard local light cone, providing a geometric latency reference across space.

**Dual-Pulse Triangulation and Geometric-Solution Algorithm**

The local-end system must collect pulse measurement data from two (or more) reference baselines simultaneously. The local end ($L_1$) performs **cross-correlation** between the quantum-entanglement event timestamp sequence it retains and the classical feature data streams transmitted from each baseline:

$$R_{AB}(\tau) = \int A_{L_1}(t) B_{L_2}(t+\tau) dt$$

By comparing the continuous feature curve matching of two or more baselines of different lengths and performing local differential reconstruction, the system eliminates the single-axis blind spot and precisely solves the projection deflection angle $\theta$ of the local clock worldline in the equivalent optical-clock geometry (this $\theta$ is not the Minkowski four-dimensional inner-product angle).

The mapping relationship between the "local geometric dilation factor relative to the ideal curvature-free trunk limit" $\Gamma_{\text{trunk}}$ and the geometric deflection angle $\theta$ is defined as:

$$\cos \theta = \frac{d\tau}{d(\mathcal{C}_{\text{trunk}} - t_0)} = \frac{1}{\Gamma_{\text{trunk}}(t)} \quad \implies \quad \Gamma_{\text{trunk}}(t) = \sec \theta \ge 1$$

This is an equivalent optical-clock geometric definition within the TCLM model, not a standard result of general relativity.

Here $\mathcal{C}_{\text{trunk}} - t_0$ is the causal-order parameter relative to the initial handshake, not a directly observable global absolute time.

When the local spacetime has no relative velocity or gravitational-potential tilt, $\theta = 0^\circ$ and $\Gamma_{\text{trunk}} = 1$ (the local time-flow rate equals the trunk limit). When curvature tilt exists, the dilation factor $\Gamma_{\text{trunk}} \approx 1 + \frac{1}{2}\theta^2$.

The "local time-flow-rate factor" $\Gamma_{\text{local}}$ in the symbol note of this chapter is the ratio of the local $\Gamma_{\text{trunk}}$ to the initial-handshake reference node $\Gamma_{\text{trunk,base}}$:

$$\Gamma_{\text{local}} = \frac{\Gamma_{\text{trunk,local}}}{\Gamma_{\text{trunk,base}}}$$

Thus $\Gamma_{\text{local}}$ may be greater than, equal to, or less than 1. DPSP local triangulation directly solves $\Gamma_{\text{trunk}}$, while the initial handshake locks $t_0$ and $\Gamma_{\text{trunk,base}}$.

This step is **purely performed locally via multi-baseline data comparison and geometric reconstruction**, without relying on real-time cross-galactic communication.

When three or more baselines of different lengths are available, a closure method can further verify the uniqueness and measurement stability of the $\theta$ solution.

In strong gravitational fields or extreme-curvature environments, the system must strictly use the exact solution $\Gamma_{\text{trunk}} = \sec \theta$ and must not use the small-angle approximation.

### 1.1 Geometric Insufficiency of a Single Baseline

In DPSP, two or more baselines of different lengths are not an engineering preference but a necessary condition for angle measurement.

A single baseline provides only a scalar timestamp difference:

$$R_{AB}(\tau) = \int A_{L_1}(t) B_{L_2}(t+\tau) dt$$

This scalar only tells the system that "some timestamp difference exists" but cannot distinguish the source of the delay:

- time-flow-rate difference
- spatial-curvature difference
- instrument-response difference
- random fluctuation

More critically: an unknown angle $\theta$, with only a single-length accumulated delay, cannot be mathematically distinguished among multiple possible solutions.

Any system attempting to solve the local geometric deflection angle with only a single baseline obtains only a single-axis scalar projection, and the solution space has rotational degeneracy. Therefore, if only one-dimensional time-flow rate is to be solved, two baselines of different lengths and collinear suffice; if two- or higher-dimensional geometric deflection angle is to be solved, at least two non-collinear baselines of different lengths are required. Length difference provides radial-delay decomposition; non-collinearity provides angle-degeneracy removal. Together they constitute the necessary condition for uniquely solving the geometric deflection angle.

### 1.2 Functional Positioning of the Single Composite Pulse and Degeneracy Removal

A traditional one-way classical optical signal provides only a scalar delay, which cannot distinguish whether the delay arises from spatial distance or time-flow-rate tilt.

The single pulse unit of this protocol is composed of a quantum-entanglement event timestamp and a classical optical return timestamp:

1. Quantum-entanglement event timestamp: recorded by the local atomic clock, unaffected by the classical propagation-path delay.
2. Classical optical return timestamp: recorded by the local atomic clock, affected by spatial distance and local curvature.

After ex-post comparison, the two can partially separate spatial propagation delay from time-flow-rate-related delay.

This function does not depend on any specific interpretation of quantum mechanics, nor does it claim that quantum entanglement can directly observe the trunk.

Under the TCLM framework, the quantum-entanglement event timestamp can at most be regarded as a second set of local measurements with a different fluctuation source from the classical optical timestamp, not the trunk itself. This correspondence is an interpretive correspondence within the framework, relying on the premise of quantum-entanglement latency, not on an experimentally confirmed physical fact.

**Key Physical Conditions and Limitations**

There are three core conditions for DPSP to hold:

First, entanglement latency and optical latency must be affected by different factors. Optical latency is affected by spatial path, propagation speed, and local curvature; what affects entanglement latency is not yet fully understood. Based on existing Bell-test experiments (e.g., Aspect 1982, Zeilinger 1998, etc.), "local hidden-variable mechanisms at or below the speed of light" have been ruled out; its mechanism is not the same as optical latency. If the two are affected by exactly the same factors, they will cancel upon subtraction and cannot be separated. If they are affected by different factors, they will not cancel upon subtraction, and partial spatial delay and time-flow-rate-related delay can be separated.

Second, entanglement latency must be sufficiently stable. If its fluctuation is too large, then after subtraction only noise remains, and no effective signal can be extracted.

Third, entanglement latency must be significantly smaller than optical latency, to serve as a stable anchor. At deep-space scales, optical latency is on the order of minutes, while entanglement latency is indistinguishable under current precision; this condition is naturally satisfied.

Under current optical-lattice-clock precision, entanglement latency is too small to be distinguished, so it can be regarded as synchronized. This is not "assuming it is synchronized," but "current precision is insufficient to detect its non-synchronization." However, whether this latency will cause observable error over long-term accumulation remains to be tested experimentally. If future experiments find that this latency varies significantly with local gravitational potential or velocity field, then other local reference events unrelated to propagation-path delay must be used.

This protocol does not need to separate the specific values of optical latency and entanglement latency; what is measured is the difference between the two timestamps recorded by the local clock for the same set of events. This difference is a combination of the two. As long as the two are affected by different factors, this combination can be decomposed into components distinguishable from optical latency.

### 1.3 Operational Independence of DPSP

DPSP's local measurement architecture does not depend on high-frequency bidirectional phase-locking, nor does it depend on the definition of absolute simultaneity. However, the second-layer initial handshake still depends on a single ephemeris and a one-way light-speed convention; this is the engineering premise for the one-time alignment constant $t_0$.

Its operational independence comes from two sources:

- Optical event timestamp: affected by propagation delay.
- Entanglement event timestamp: a local record, unaffected by geometric-path delay; but its pairing relationship with the optical event still needs to be confirmed ex-post via a classical channel, without involving faster-than-light communication.

Unless otherwise specified below, $\Delta t_{\text{latency}}$ adopts the local clock-difference definition, i.e.:

$$\Delta t_{\text{latency}} \equiv \Delta\tau_{\text{local}} = t_{\text{light}} - t_{\text{entanglement}}$$

where both $t_{\text{light}}$ and $t_{\text{entanglement}}$ are local atomic-clock readings. Layer-1 triangulation solves $\Gamma_{\text{trunk}}$, which is then converted with the initial-handshake reference $\Gamma_{\text{trunk,base}}$ to obtain $\Gamma_{\text{local}}$.

If the local clock difference $\Delta\tau_{\text{local}}$ needs to be converted to the initial-handshake reference, then under reference normalization:

$$\Delta t_{\text{latency}}^{(\text{base})} = \frac{\Delta\tau_{\text{local}}}{\Gamma_{\text{local}}}$$

Unless otherwise superscripted, $\Delta t_{\text{latency}}$ always refers to the local clock-difference version.

The initial value $t_0$ is a conventional integration constant; all subsequent quantities are causal-order reconstructions relative to $t_0$.

This independence relies on the operational premise described in Section 1.2; this premise is not a necessary condition for DPSP to hold, but its precision remains to be further tested experimentally.

---

### 2. Layer 2: Interplanetary Initial-Handshake Pulse (Deep-Space Initial-Constant Locking)

Because the global causal-order reconstruction equation necessarily contains an unknown **initial integration constant ($t_0$)**, solving the local $\Gamma(t)$ variation alone yields only the time-advance quantity, not the initial alignment constant between the two time axes.

- **Single-handshake procedure**:
  1. The reference end (e.g., Earth) emits a single classical deep-space radio pulse carrying the initial timestamp $t_{\text{Earth\_start}}$ to the target end (e.g., Mars).
  2. The Mars end receives this pulse and, combining orbital geometric distance and multi-frequency dispersion compensation, computes the light-speed delay $\Delta t_{\text{propagation}}$, thereby establishing the initial alignment relationship between Mars local time and Earth reference time ($t_0$).

- **Autonomous-computation state**:
  Once the initial value $t_0$ is locked, the Mars end can cease high-frequency deep-space communication and rely purely on the $\Gamma_{\text{local,Mars}}(\tau)$ obtained in real time from "Layer-1 local triangulation" to independently perform causal-order autonomous reconstruction relative to the initial handshake:

  $$\mathcal{C}_{\text{trunk\_reconstructed}}(\tau) = t_0 + \Gamma_{\text{trunk,base}}\int_{\tau_0}^{\tau} \Gamma_{\text{local,Mars}}(\tau')\, d\tau'$$

  where $\Gamma_{\text{trunk,base}}$ is also locked by the initial handshake. If the reference node is defined as curvature-free and normalized to $\Gamma_{\text{trunk,base}}=1$, this factor degenerates to 1, and the formula reduces to $\mathcal{C}_{\text{trunk\_reconstructed}}(\tau) = t_0 + \int_{\tau_0}^{\tau} \Gamma_{\text{local,Mars}}(\tau')\, d\tau'$.

- **Blackout re-synchronization mechanism**:
  If a deep-space node enters a long-term communication blackout due to solar occultation, the local continuous-field integration engine can still independently track time-flow-rate variation without causing a causal-order discontinuity. However, the $t_0$ locked by the initial handshake is a one-time classical alignment parameter; it does not drift due to local integration. The purpose of re-handshaking after blackout is to re-confirm the alignment relationship between the two time axes and to correct engineering errors possibly accumulated during local integration. The geometric curvature measurement of the time-flow rate itself does not fail due to communication interruption.

---

### 3. Layer 3: Continuous Rate Dynamic Control (Adaptive Pacing, Quadratic Compensation, and Causal Backpressure)

To address the frequency asymmetry and data-queue overflow problems arising from the continuously fluctuating time-flow rate ($\frac{d\Gamma}{dt} \neq 0$), the protocol introduces the following dynamic control mechanisms:

- **Adaptive Pulse Frequency Scaling**:
  The two ends exchange their respective local time-flow-rate curves $\Gamma_{\text{local}}(t)$ during the initial handshake. The local end can then combine its own $\Gamma_{\text{local,source}}(t)$ with the received $\Gamma_{\text{local,target}}(t)$ to reconstruct the relative flow-rate ratio $\lambda(t) = \frac{d\tau_{\text{target}}}{d\tau_{\text{source}}}$. The high-rate end (source) automatically adjusts its timekeeping pulse emission period:
  $$\Delta t_{\text{source}} = \frac{\Delta \tau_{\text{target}}}{\lambda(t)}$$
  When the target end is in a low-rate region ($\lambda \ll 1$), the source automatically lengthens its emission interval to match the target's local processing frame rate, avoiding high-frequency pulse bombardment of the low-rate end.

- **Continuous Curvature Quadratic Compensation**:
  In a continuously varying gravitational or acceleration field, the dual-pulse signal header is forced to carry the node's current "local time-rate acceleration and gravitational-gradient derivative ($\frac{d\Gamma_{\text{local}}}{d\tau}$)." The receiving end uses a Taylor-expansion quadratic term for continuous curvature fitting:
  $$\Gamma_{\text{local}}(\tau + \Delta \tau) \approx \Gamma_{\text{local}}(\tau) + \frac{d\Gamma_{\text{local}}}{d\tau} \Delta \tau + \frac{1}{2}\frac{d^2\Gamma_{\text{local}}}{d\tau^2} (\Delta \tau)^2$$
  The receiving end can thus locally predict the clock drift between two discrete pulses without relying on high-frequency pulses, resolving the accumulated phase error caused by continuous acceleration fields.

  Phase perturbations from the solar wind and interplanetary plasma can be regarded as quasi-common-mode for all nodes within the solar system, but not strictly common-mode. Through multi-node cross-comparison and differential computation, some of these background perturbations can be partially suppressed without establishing precise individual models.

  It should be noted that continuous curvature quadratic compensation is intrinsically a discrete-sampling system. When the gravitational-field variation frequency approaches or exceeds the pulse-sampling frequency, aliasing occurs, and the sampling cannot resolve the variation. This is a physical limit of all discrete-sampling systems, not a design flaw of this protocol. In practice, higher sampling rates, adaptive triggering mechanisms, or a priori gravitational-field models must be used; the specific engineering response is left to subsequent engineering teams.

- **Causal Backpressure and Queue Mechanism**:
  When the flow-rate ratio between source and target suddenly changes drastically (e.g., the target suddenly enters a strong gravitational well), causing the target's local causal-processing rate to lag behind the upstream input rate, the target's ingress queue triggers a critical backpressure signal.
  * The signal forces upstream nodes to reduce data-transmission throughput.
  * Overloaded event data is temporarily stored in the local node's "Causal Buffer," queued according to the monotonicity constraint $\frac{d\mathcal{C}_{\text{trunk}}}{d\tau} > 0$.
  * Messages are stretched for transmission in the delay pipeline; provided the buffer capacity is sufficient, buffer overflow or event loss is avoided for any low-rate sub-branch due to time dilation.

  This buffer is a local node engineering-queue mechanism whose capacity is constrained by the node hardware and local causal-processing rate. $J^{\text{cap}}$ is a parameter in the theoretical model characterizing the local node's information-throughput limit; its precise correspondence to the actual engineering buffer is left to subsequent engineering teams.

- **High-Rate Inertial Bridging**:
  The DPSP dual-pulse is a discrete sampling; between two measurements, there is an observation blind zone for the variation of $\Gamma_{\rm local}(t)$. To reduce aliasing and improve continuous-compensation accuracy, the node may optionally be equipped with a high-sampling-rate accelerometer (or IMU) that continuously outputs the intrinsic acceleration time series.

  This signal does not directly give $\Gamma_{\rm local}$, but can serve as a high-frequency bridging observation between two discrete DPSP measurement points, for:
  - estimating $\frac{d\Gamma_{\rm local}}{d\tau}$ and $\frac{d^2\Gamma_{\rm local}}{d\tau^2}$, strengthening the continuous curvature quadratic compensation;
  - detecting drastic dynamic changes within the pulse interval, triggering adaptive additional measurement or increasing the subsequent sampling rate;
  - cross-correlation or consistency constraints with the $\Gamma_{\rm local}$ sequence solved by the dual-pulse.

  Note: According to the equivalence principle, intrinsic acceleration cannot by itself distinguish gravitational from kinematic acceleration, nor can it directly measure gravitational-potential differences. Its role is to fill the discrete-sampling blind zone as an auxiliary observation, not to replace dual-pulse geometric solving.

---

### 4. Theoretical Closure and Engineering-Boundary Decoupling

- **Theoretical Resolution Limit**: After removing medium and geometric perturbations, the theoretical resolution of this protocol under a geometric closed loop is constrained by the hardware limit of current optical-lattice clocks. In terms of fractional frequency stability, the current level has reached the $10^{-18}$ to $10^{-19}$ order of magnitude; when integrated over 1 day, this corresponds to an absolute time error of approximately $10^{-13}$ to $10^{-14}\text{ s}$. This is the hardware resolution limit, not a solo contribution of the protocol.

- **Deep-Space Engineering Error Budget**: In a real deep-space environment, radio signals are disturbed by solar-wind ionospheric plasma dispersion, solar gravitational-lensing effects, and celestial ephemeris uncertainties (uncompensated uncertainty can reach the $\sim 10^{-6}$ to $10^{-8}\text{ s}$ level). Note that there is a gap of about four to five orders of magnitude between the hardware resolution of current optical-lattice clocks (in fractional frequency stability, currently at the $10^{-18}$ to $10^{-19}$ order) and the engineering alignment precision achievable by deep-space links ($\mathcal{O}(10^{-9}\text{ s})$). This gap mainly arises from deep-space radio-link signal-to-noise attenuation, plasma-dispersion residuals, and ephemeris uncertainties, and constitutes the primary engineering challenge during physical deployment. This paper only provides the theoretical framework and error budget; the specific link-engineering correspondence is left to subsequent engineering teams.

---

## Chapter 4: Astrophysical-Measurement Data Calibration and Earth–Mars Transfer Example

(Note: The $\gamma_{B/A}$ used in this chapter is defined as the **relative** time-rate variation between two physical observation endpoints, and must be strictly distinguished from the local time-flow-rate factor $\Gamma_{\text{local}}$ relative to the initial handshake in Chapter 3.)

### 1. Surface and GPS Satellite Regional Calibration Case (Earth Calibration)

Considering the combined special- and general-relativistic effects in low-Earth orbit (velocity slows by 7 μs/day, gravitational potential speeds by 45 μs/day), the measured net drift rate between the surface reference end and the GPS branch end is +38 μs/day. Substituting into the two-endpoint relative rate-variation formula:

$$\gamma_{\text{GPS/Earth}} = \frac{d\tau_{\text{GPS}}}{d\tau_{\text{Earth}}} \approx 1 + 4.40 \times 10^{-10}$$

This data serves purely as a calibration example for "single-point rate variation can be measured and reconstructed" within a regional gravity well.

### 2. Earth–Mars Interplanetary Docking and Worldline Path-Integration Calibration

Let the Earth geoid and the Mars surface be independent physical branch endpoints. According to the complete calculation of NIST Ashby & Patla (2025), the Mars atomic clock averages about 477 μs per day faster than the Earth geoid, with a ±226 μs/day variation with orbital eccentricity.

**This model uses continuous worldline field integration as the primary dynamic-alignment core.** All time-flow rates are intrinsically continuously floating dynamic fields; the previously named "local static chain-transfer law (e.g., $\gamma_{C/A} = \gamma_{C/B} \cdot \gamma_{B/A}$)" is merely a discrete special case to which the integral operation naturally degenerates when the gravitational-potential perturbation tends to zero.

In relay communication, the satellite serves only as an "engineering signal-forwarding (edge-router)" function and does not constitute a necessary intermediary node for physical causal computation. The Mars end needs only to receive the single initial-handshake pulse from Earth; combined with the Layer-3 dynamic pacing and backpressure mechanisms, it can perform autonomous reconstruction via local triangulation and continuous integration. Under given mission-geometry, sampling-rate, and multi-frequency dispersion-compensation assumptions, taking a local 100 s continuous-field integration window as an example (not two-way link delay), the engineering alignment error-budget target is at the nanosecond level; related error sources and magnitudes are given in Chapter 3, Section 4. This is a budget target, pending end-to-end link simulation and empirical validation. The theoretical limit is constrained by the optical-lattice-clock hardware, not achieved by the protocol alone. The actual integration-window length depends on mission geometry and link conditions.

| Error Source | Uncompensated Magnitude | Compensated Residual |
|:---|:---|:---|
| Plasma dispersion | $\sim 10^{-6}\text{ s}$ | $\sim 10^{-10}\text{ s}$ (multi-frequency compensation) |
| Ephemeris uncertainty | $\sim 10^{-8}\text{ s}$ | $\sim 10^{-9}\text{ s}$ |
| Signal-to-noise attenuation | Depends on link | Depends on link |
| Integration-window accumulation | Depends on window length | Depends on window length |
| Clock hardware limit (fractional frequency stability) | $10^{-18}$ to $10^{-19}$ order | $10^{-18}$ to $10^{-19}$ order |

This table is only an order-of-magnitude illustration; specific values remain pending end-to-end link simulation and empirical validation.

---

## Chapter 5: Future Extension Concepts (Unverified Capabilities): Gravitational-Wave Response Exploration Based on Dual-Pulse Timing Networks

1. **Spacetime-Perturbation Response (Conceptual)**: If a dual-pulse dynamic-curvature-solving endpoint network (e.g., an Earth–Mars timing network) is operated over the long term, its solved $\Gamma_{\text{local}}(t)$ curve may, in principle, not only reflect regular orbits and gravitational potential but also exhibit transient distortions in response to gravitational waves (metric perturbation, $h_{\mu\nu}$) sweeping through the local spacetime. This is a conceptual expectation, currently without a complete response function or sensitivity model.

2. **Chronometric Gravitational-Wave Sensing (Early Concept)**: A long-term multi-node $\Gamma_{\text{local}}(t)$ monitoring network may, under noise conditions and instrument-stability allowances, in principle respond to spacetime perturbations (including gravitational waves) sweeping through the region. This direction is worth exploring as one future possible application; however, no complete sensitivity, noise-spectrum, frequency-band, or integration-time budget currently exists. It is an early concept highly dependent on actual noise-suppression effectiveness, not a verified capability of this protocol.

This paper does not claim that this network already has gravitational-wave detection capability, nor does it claim that it can replace or surpass existing interferometers. This chapter is only a conceptual discussion of a future research direction.

---

## Chapter 6: Theoretical and Engineering Pressure Tests and Boundary Defenses (Comprehensive Q&A)

| No. & Question | Answer & Boundary Defense |
| :--- | :--- |
| **Q1: How to explain the permanent time difference of the "twin paradox"?** | In the TCLM framework, the two atomic clocks experience different spatial-motion trajectories (acceleration and gravitational fields); their accumulated branch curvature delays are inherently unequal. This is a curvature difference of geometric branches, not a causal reversal on the trunk. |
| **Q2: If FTL holds, can signals be sent to the past or causal reversal be realized?** | Under the TCLM postulates, no. Pure geometric acceleration can only produce apparent reverse-order reception of wavefront signals ($\Delta t_{\text{latency}} > 0$) and cannot reverse the causal vector within a single manifold. The global topological causal operator is set to be strictly positive-definite ($\operatorname{sgn}(\mathcal{C}) \equiv +1$); historical coordinates are, within the model, topologically irreversible states. Therefore, under the TCLM model, sending information to the past or causing a grandfather paradox is not permitted; however, this paper does not claim to have proved the existence of any FTL mechanism. |
| **Q3: After matter falls into a black-hole event horizon, does time stop or flow backward?** | Under TCLM's topological causal structure, not necessarily. The black-hole event horizon is only a geometric gateway where branch curvature reaches its limit; within the model, the evolution of matter on the causal trunk is still set to be strictly forward. The observable time near the event horizon and external-observer readings still require separate modeling and cannot be directly inferred from the causal order of the trunk alone. |
| **Q4: Does the TCLM causal order break tensor covariance?** | No. TCLM distinguishes "geometric observables" from "topological causal order." Local geometric observables (e.g., clock tick rate $d\tau$ and geometric latency $\Delta t_{\text{latency}}$) obey Lorentz covariance and the general-relativistic metric equation (as a local effective field theory). $\mathcal{C}_{\text{trunk}}$ serves only as a causal-sorting index of the global topological directed acyclic graph (DAG) and does not interfere with the metric-tensor operation of any local inertial frame. |
| **Q5: Does the TCLM framework face the relativity limit of "mass-energy divergence near the speed of light"?** | This paper does not claim to have resolved this limit. Type A (relative-distance FTL) and Type B (discrete FTL / topological transition, see Appendix A) are merely phenomenological classifications under the TCLM framework, used to explain "if some FTL mechanism exists, how the causal direction is maintained by the model." This paper does not claim that Type A or Type B already has engineering feasibility, nor does it claim that the mass-energy divergence limit has been bypassed. |
| **Q6: Is TCLM a disguised revival of Newtonian "absolute spacetime" or the "ether"?** | No. Newtonian absolute spacetime presupposes a "global absolute clock ticking synchronously at all points" and a rigid spatial medium. TCLM's $\mathcal{C}_{\text{trunk}}$ is not a global synchronized clock but a second-parameterized index of causal chronological order. Its strict monotonic increase guarantees only the causal direction; it does not provide an observable privileged simultaneity slice. The chronological order of $\mathcal{C}_{\text{trunk}}$ is only a mathematical index of causal order; it does not constitute a physically observable simultaneity plane. TCLM also does not introduce a mechanical ether or a preferred reference frame. Under the TCLM framework, all physically measured time (clock time) is a geometric path integral on the branch manifold. |
| **Q7: Does the non-local correlation of quantum-entanglement measurement violate the no-communication theorem or cause trunk disorder?**<br>(Its non-locality has been confirmed by Bell tests; see Chapter 3, Section 1.2.) | No. In this protocol, quantum entanglement serves only as one local measurement event within each pulse unit, recorded by the local atomic clock as an event timestamp. This timestamp is compared ex-post with the classical optical return timestamp. The dual-pulse itself relies on two or more independent baselines, rather than using quantum entanglement for real-time communication. Single-sided measurement yields only random eigenvalues and cannot immediately read the opposite end's time; the system uses ex-post comparison of the two timestamps to solve the geometric deflection angle locally, without relying on controllable FTL information transfer, and at the operational level does not conflict with the no-communication theorem. |
| **Q8: Will continuous rate variation and drastic flow changes cause DPSP to crash?** | Under normal mission geometry and sampling density, the design goal is not to crash; but this is a design goal, not a guarantee. The protocol has introduced adaptive pulse pacing, continuous curvature quadratic compensation, and causal backpressure buffering to maintain data-topological integrity and queue safety under continuous acceleration and extreme flow-rate differences. However, if the gravitational-field variation frequency approaches or exceeds the pulse-sampling frequency, aliasing occurs and the sampling cannot resolve the variation; if outside the design envelope, the protocol may still fail. This is a physical limit of discrete-sampling systems, requiring higher sampling rates or a priori model support. |

---

## Chapter 7: Conclusion

This paper attempts to deconstruct the problem of special relativity exceeding the real domain at extreme speeds as "apparent reverse-order reception of wavefront signals," and proposes the formal framework of "topological causal trunk" and "geometric branch curvature" in TCLM, as well as the "Dual-Pulse Synchronization Protocol (DPSP)" and its underlying rate-variation algorithm as a conceptual operational framework for engineering implementation.

The model uses "spacetime worldline continuous-field integration" as its principal dynamic core working hypothesis. The measured value of GPS (+38 μs/day) and the NIST-computed value of the Earth–Mars system (477 μs/day) can serve as input calibration cases for relativistic time rates, matching in order of magnitude the dynamic gravity-well and non-inertial-frame rate variations required by the protocol; however, this is input calibration, not empirical verification of the protocol's autonomous reconstruction. The protocol's autonomous reconstruction of the causal order relative to the initial handshake under dynamic environments remains theoretical, pending end-to-end simulation and empirical validation.

In terms of precision, this paper clearly distinguishes two levels:

1. **Hardware Resolution Limit**: The local resolution of current optical lattice clocks has reached the $10^{-18}$ to $10^{-19}$ order of magnitude, which is a theoretical upper bound of hardware capability, not a solo contribution of the protocol.
2. **Engineering Alignment Error Budget**: In the Earth–Mars case, after multi-frequency dispersion compensation and dynamic metric-field fitting, the alignment error-budget target relative to the initial handshake reference is at the nanosecond level ($\mathcal{O}(10^{-9}\text{ s})$). This is a budget target; only if subsequent end-to-end simulation and empirical validation pass, may it satisfy the stringent requirements of interplanetary deep-space navigation and communication. Cross-galactic scales are a logical extension whose error budget requires separate modeling.

Furthermore, whether this protocol may extend to a distributed "chronometric gravitational-wave response network" research direction remains an early concept without sensitivity and noise-budget assessment. This paper does not claim that it can replace or supplement existing interferometers, nor does it claim that it possesses gravitational-wave detection capability.

This paper primarily addresses two things:

1. **Re-characterization of a mathematical boundary**: The Lorentz transformation yields imaginary (complex) values when $v > c$, which should be understood as "the mathematical model exceeding its real domain," not "the physical flow of time backward."
2. **Proposal of a measurement method**: The Dual-Pulse Synchronization Protocol (DPSP), which uses ex-post comparison of optical-event timestamps (affected by spatial path and local curvature) and entangled-event timestamps (whose mechanism differs from optical latency; Bell tests have ruled out local hidden-variable mechanisms at or below the speed of light) to separate spatial latency from local time-flow rate.

The remaining chapters serve as engineering calibration, extended applications, and boundary defenses, and do not constitute claims regarding the existence of FTL, gravitational-wave detection capability, FTL quantum-entanglement communication, or the engineering feasibility of cross-galactic scales.

Conceptually, TCLM's causal tree attempts to provide a coexisting path for Newton's and Einstein's views on time.

---

## Appendix A: Conditional Phenomenological Remarks: Apparent Effects Within the TCLM Framework If Some Class of FTL Mechanism Exists (Not an Engineering Necessity, and Not a Claim for the Existence of FTL)

1. **Conditional Inference 1: Apparent Time-Axis Decoupling and "Apparent Reverse-Order" Observation**

   * **Hypothetical Situation**: If some class of FTL entity or FTL wavefront exists and is described within the TCLM framework as moving toward an observer, then under that model the observer may "first see the arrival image, then receive photons from the origin and midpoint."

   * **Dual-Track Path Mechanism (Model-Internal Classification)**:

     * **Type A (Relative-Distance FTL)**: The rate of increase of the proper distance between two points exceeds $c$ due to changes in the spatial geometry itself. A typical example is that under cosmic expansion, sufficiently distant galaxies recede at speeds exceeding the speed of light. This is a rate of change of relative distance, not an intrinsic speed of an object exceeding $c$ in its local reference frame; it does not involve local FTL motion and does not violate causality. This mechanism can also be equivalently described as "space flow carrying an object": the variation of the metric simultaneously determines the change of distance and the direction of space flow — two languages for the same geometric fact. If the distribution of $T_{\mu\nu}$ can be actively constructed, then in theory the local distance field can be changed; here "theoretically realizable" means that the general-relativistic field equation permits a corresponding mathematical solution, without involving whether the $T_{\mu\nu}$ required by that solution can be constructed from known forms of matter or energy.

     * **Type B (Discrete FTL / Topological Transition, Model-Internal Assumption)**: This type currently has no observational case and is purely a model-internal inference. If realized via a topological jump isomorphic to the "quantum tunneling effect," then under that model the observer may experience a "Discontinuous Frame": the old image at point A has not yet faded, and a new image at point B bursts into existence instantaneously, possibly accompanied by a single high-energy spacetime-metric perturbation radiation.

   * **Causal Defense (Model-Internal)**: Such phenomena are classified in TCLM as apparent wavefront reverse-order reception on geometric branches. On the topological trunk, event settlement is set to be strictly monotonically increasing. Under this speculative model, the observer may receive some future image signals in advance, but this does not constitute substantive interference with the event ontology, nor does it permit sending information to the past; the grandfather paradox is not permitted within this model. This paper does not claim that any such FTL mechanism exists or is feasible.

2. **Conditional Remark 2: Read-Only Causal Horizon at the Extreme-Speed Limit (Model-Internal Concept)**

   * Under such assumptions, when a carrier approaches and exceeds the speed of light, its geometric branch curvature enters an extreme high-pressure region. Any operation attempting to return a "dynamic control command (write)" to the upstream trunk is, within the model, set as non-writable.
   * Under this speculative model, such a carrier can only play a passive-observer role and cannot become a tool for causal reversal. This paragraph does not constitute a claim regarding FTL engineering feasibility.

## Associated Notes

Lee Wang Hin (2026). *The Circular Reasoning in the Superluminal Ban: A Logical Note on the Einstein Synchronization Convention.* Zenodo. DOI: 10.5281/zenodo.22782047