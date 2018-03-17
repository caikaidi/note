# Physics of Semiconductor Device

## 1. Electrons and Holes in Semiconductors

### 1.1 Silicon Crystal Sturcture

- unit cell
- lattice constant
- primitive cell
- Miller indices

### 1.2 Bond Model of Electrons and Holes

### 1.3 Energy Band Model

- energy bands
- valence band
- conduction band
- band gap

#### 1.3.1 Energy Band Diagram

| Semiconductor | Ge   | Si   | GaAs |
| ------------- | ---- | ---- | ---- |
| $E_g$         | 0.67 | 1.12 | 1.42 |

### 1.3.2 Donors and Acceptors in the Band Model

- shallow levels
- deep levels

### 1.4 Semiconductors, Insulators, and Conductors

$E_g\sim 4$eV

### 1.5 Electrons and Holes

> We may think of holes as bubbles in liquid, floating up in the energy band. Similarly, one may think of electrons as water drops that tend to fall to the lowest energy states in the energy band.

#### 1.5.1 Effective Mass

$$
\text{Acceleration}=\frac{q\varepsilon}{m_p}=-\frac{q\varepsilon}{m_n}
$$

|       | Si   | Ge   | GaAs  |
| ----- | ---- | ---- | ----- |
| $m_n$ | 0.26 | 0.12 | 0.068 |
| $m_p$ | 0.39 | 0.30 | 0.50  |

$$
\text{Acceleration}=-\frac{q\varepsilon}{\hbar^2}\frac{\mathrm d ^2 E}{\mathrm d \vec k^2}\\
\text{Effective mass}=\frac{\hbar^2}{\mathrm d^2 E/\mathrm d \vec k^2}
$$

#### 1.5.2 How to Measure the Effective Mass

- cyclotron resonance

### 1.6 Density of States

$$
D_C(E)=\frac{\text{number of states in }\Delta E}{\Delta E\times\text{volume}}\\
D_C(E)=\frac{8\pi m_n\sqrt{2m_n(E-E_C)}}{h^3},E\ge E_C\\
D_V(E)=\frac{8\pi m_p\sqrt{2m_p(E_V-E)}}{h^3},E\le E_v\\
$$

### 1.7 Thermal Equilibrium and the Fermi Function

#### 1.7.1 An Analogy for Thermal Equilibrium

> Every energy state in the conductino and valence bands has a certain probability of being occupied by an electron.

#### 1.7.2 Fermi Function—The Probability of an Energy State Being Occupied by an Electron

Fermi-Dirac Distribution Function:
$$
f(E)=\frac 1 {1+\exp[(E-E_F)/KT]}
$$
Maxwell-Boltzmann approximation:
$$
f(E)\approx \exp[-(E-E_F)/kT],E-E_F\gg -kT\\
1-f(E)\approx \exp[-(E_F-E)/kT], E-E_F\ll -kT
$$

### 1.8 Electron and Hole Concentrations

#### 1.8.1 Derivation of *n* and *p* from *D(E)* and *f(E)*

electron concentration
$$
\begin{align}
n&=\int_{E_c}^{\text{Top of conduction band}}f(E)D_C(E)\mathrm d E\\
&=N_C\exp[-(E_C-E_F)/kT]
\end{align}
$$
hole concentration
$$
\begin{align}
p&=\int_{\text{bottom of valence band}}^{E_V}D_V(E)(1-f(E))\mathrm d E\\
&=N_V\exp[-(E_F-E_V)/kT]
\end{align}
$$

$$
N_C=2\left[\frac{2\pi m_nkT}{h^2}\right]^{3/2}\\N_V=2\left[\frac{2\pi m_pkT}{h^2}\right]^{3/2}
$$

|       | Ge                   | Si                   | GaAs                |
| ----- | -------------------- | -------------------- | ------------------- |
| $N_C$ | $1.04\times 10^{19}$ | $2.8\times 10^{19}$  | $4.7\times 10^{17}$ |
| $N_V$ | $6.0\times 10^{18}$  | $1.04\times 10^{19}$ | $7.0\times 10^{18}$ |

$N_C$: effective density of states of the conduction band

$N_V$: effective density of states of the valence band

#### 1.8.2 Fermi Level and the Carrier Concentrations

$$
E_C-E_F =kT\cdot\ln(N_C/n)\\
E_F-E_V=kT\ln(N_V/p)
$$

#### 1.8.3 The *np* Product and the Intrinsic Carrier Concentration

$$
np=N_CN_V\exp[-E_g/kT]\\
np=n_i^2\\
n_i=\sqrt{N_CN_V}\exp[-E_g/2kT]
$$

If there are no dopants present, the semiconductor is said to be **intrinsic**.

In an intrinsic semiconductor, $n=p=n_i$. Therefore, $n_i$ is called the **intrinsic carrier concentration**.

- majority carriers
- minority carriers

In an intrinsic semiconductor, the Fermi level is nearly at the middle of the band gap. This level is called the **intrinsic Fermi level**, $E_i$.
$$
n_i=N_C\exp[-(E_C-E_i)kT]\\
E_i=E_C-E_g/2-kT\ln\sqrt{\frac{N_C}{N_V}}
$$

### 1.9 General Theory of *n* and *p*

Since $E_d$ is usually a few $kT$ above $E_F$, we say that nearly all the donor atoms are ionized. Similarly, all the acceptor atoms are ionized.

Charge neutrality requires that
$$
n+N_a=p+N_d
$$

- $N_d-N_a\gg n_i$(i.e., N type)
  $$
  n=N_d-N_a\\
  p=n_i^2/n
  $$

- $N_a-N_d\gg n_i$(i.e., P type)
  $$
  p=N_a-N_d\\
  n=n_i^2/p
  $$


### 1.10 Carrier Concentrations at Extremely High and Low Temperatures

At very high temperatures, it is possible to have $n_i\gg |N_d-N_a|$. The semiconductor becomes "intrinsic".

At very low temperatures, $E_F$ may rise above $E_d$, and most of the donor or acceptor atoms can remain nonionized. This phenomenon is called **freeze-out**. In this case, we have
$$
n=\left[\frac{N_CN_d}{2}\right]^{1/2}\exp[-(E_C-E_d)/2kT]
$$

## 2. Motion and Recombination of Electrons and Holes

### 2.1 Thermal Motion

$$
\text{Average electron kinetic energy}=\frac{\int f(E)D(E)(E-E_C)\mathrm d E}{\int f (E)D(E)\mathrm d E}=\frac 32kT
$$

Thermal velocity
$$
V_{th}=\sqrt{\frac{3kT}{m}}\sim10^7\text{cm/s}
$$
The mean free time is typically $10^{-13}$s. The distance between collisions is a few tens of nanometers.

### 2.2 Drift

#### 2.2.1 Electron and Hole Mobilities

Hole mobility $\mu_p$
$$
\nu = \mu_p\varepsilon\\
\mu_p=\frac{q\tau_{mp}}{m_p}
$$
Electron mobility $\mu_n$
$$
\nu=-\mu_n\varepsilon\\
\mu_n=\frac{q\tau_{mn}}{m_n}
$$

|         | Si   | Ge   | GaAs |
| ------- | ---- | ---- | ---- |
| $\mu_n$ | 1400 | 3900 | 8500 |
| $\mu_p$ | 470  | 1900 | 400  |

#### 2.2.2 Mechanisms of Carrier Scattering

- phonon scattering
  $$
  \mu_{ph}=\frac{q\tau_{ph}}{m^*}\\
  \mu_{\text{phonon}}\propto \tau_{ph}\\
  \propto\frac1{\text{phonon density}\times\text{carrier thermal velocity}}\\
  \propto\frac1{T\cdot T^{1/2}}\propto T^{-3/2}
  $$

- ionized impurity scattering
  $$
  \mu_{\text{impurity}}\propto \frac{T^{3/2}}{N_a+N_d}
  $$




$$
\frac 1\tau=\frac1 {\tau_{\text{phonon}}}+\frac 1 {\tau_{\text{impurity}}}\\
\frac 1\mu =\frac1 {\mu_\text{phonon}}+\frac1 {\mu_\text{impurity}}
$$

Velocity Saturation: electron and hole velocities saturate at around $10^7$cm/s and do not increase no matter how large $\varepsilon$ is. The culprit is **optical phonon scattering**. When the kinetic energy of a carrier exceeds the optical phonon energy $E_{opt}$, it generates an optical phonon and loses the kinetic energy. Therefore, the velocity does not rise above **saturation velocity**, $\nu_{sat}$.
$$
\frac12m^*\nu_{sat}^2=E_{opt}\Rightarrow \nu_{sat}=\sqrt{\frac{2E_{opt}}{m^*}}
$$
When we deal with devices whose sizes are smaller than the mean free path, the scattering is about to disappear. That is called **ballistic transport**.

#### 2.2.3 Drift Current and Conductivity

$$
J_{p,drift}=qp\nu=qp\mu_p\varepsilon\\
J_{n,drift}=-qn\nu=qn\mu_n\varepsilon\\
J_{drift}=J_{n,drift}+J_{p,drift}=(qn\mu_n+qp\mu_p)\varepsilon\\
\sigma=qn\mu_n+qp\mu_p
$$

$\sigma$ Is the quantity in the parentheses, called the **conductivity**. Its reciprocal is the **resistivity**, $\rho$.

### 2.3 Diffusion Current

$$
J_{n,diffusion}=qD_n\frac{\text d n}{\text d x}\\
J_{p,diffusion}=-qD_p\frac{\text d p}{\text d x}\\
$$

$D$ is called the **diffusion constant**.
$$
J_n = J_{n,dirft}+J_{n,diffusion}=qn\mu_n\varepsilon+qD_n\frac{\text d n}{\text d x}\\
J_n = J_{n,dirft}+J_{n,diffusion}=qp\mu_p\varepsilon-qD_p\frac{\text d p}{\text d x}\\
J=J_n+J_p
$$

### 2.4 Relation Between the Energy Diagram and v, $\varepsilon$ 

When a voltage is applied across a piece of semiconductor, it alters the band diagram.
$$
E_C(x)=\text{constant}-qV(x)
$$

The constant takes care of the zero references for $E_cC$ and $V$, which is unspecified and inconsequential.

The electric field
$$
E(x)=-\frac{\text d V}{\text d x}=\frac1q \frac{\text d E_C}{\text d x}=\frac1q \frac{\mathrm d E_V}{\text d x}
$$

### 2.5 Einstein Relationship Between *D* and $\mu$

$$
D_n=\frac{kT}q\mu_n\\
D_p=\frac{kT}{q}\mu_p
$$

The electron drift and diffusion currents will perfectly cancel each other out for an arbitrary doping profile.

### 2.6 Electron-Hole Recombination

Denote **excess carrier concentrations** by $n'$ and $p'$.

If the light is suddenly turned off, there will be **recombination**. The time constant of decay is called the **recombination time ** or **carrier lifetime**, $\tau$.
$$
\frac{\mathrm d n'}{\mathrm  d t}=-\frac{n'}\tau=-\frac{p'}\tau
$$
The recombination rate is proportional to excess carrier concentrations:
$$
\text{Recombination rate }=\frac{n'}\tau=\frac{p'}\tau
$$
$\tau$ has the dimension of time range from 1 ns to 1 ms, depending on the density of trace metal impurities, which cause energy levels deep in the band gap. These **deep traps** or **recombination centers** can capture electrons or holes to facilitate recombination. Another recombination process, **direct recombination**, or **radiative recombination**, is very inefficient in **indirect gap semiconductors** and very efficient in **direct gap semiconductors**.

### 2.7 Thermal Generation

The reverse process of recombination is called **thermal generation**.

When $np>n_i^2$, there is net recombination; when $np<n_i^2$, there is net generation.

### 2.8 Quasi-Equilibrium and Quasi-Fermi levels

$$
n=N_C\exp[-(E_C-E_{Fn})/kT]\\
n=N_V\exp[-(E_{Fp}-E_V)/kT]\\
$$

The condition that $n'$ and $p'$ are much less than the majority carrien conentration is commonly assumed and is called **low-level injection**.