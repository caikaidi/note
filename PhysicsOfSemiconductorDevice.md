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

#### 1.3.2 Donors and Acceptors in the Band Model

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
  \mu_{\text{impurity}}\propto \frac{T^{3/2}}{N_a+N_d}\\
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

## 3. Device Fabrication Technology

### 3.1 Introduction to Device Fabrication

- planar technology

### 3.2 Oxidation of Silicon

- dry oxidation
- wet oxidation
- horizontal furnace
- vertical furnace

### 3.3 Lithography

(**Photolithography** or **optical lithography**)

- photoresist
  - negative resists
  - positive resists
- photomask
- resist strip
- lithography field
- stepper
- optical proximity correction
- phase-shift photomask

#### 3.3.1 Wet Lithography

Fill the gap between the lens and the wafer with water is called **wet lithography** or **immersion lithography**.

#### 3.3.2 Electron Lighography

Electron-beam lithography has long been used to fabricate the photomasks used in optical lithography and for EUVL (extreme UV lithography).

#### 3.3.3 Nanoimprint

### 3.4 Pattern Transfer-Etching

- wet etching (isotropic)
- dry etching (Aniostropic) (plasma etching) (reactive-ion etching RIE)
- end-point detector
- plasma process-induced damage / wafer charging damage
- antenna effect

### 3.5 Doping

dopant profile:
- predeposition
  - ion implantation
  - gas-source doping
  - solid-source diffusion
- drive-in diffusion

#### 3.5.1 Ion Implantation

- anneal
- dopant activation

$$
N(x)=\frac{N_i}{\sqrt{2\pi}(\Delta R)}\cdot\exp[-(x-R)^2/2\Delta R^2]
$$

$N_i$ called the **implantation dose**. *R* called the **implantation range**, and $\Delta R$ called **implantation straggle**.

#### 3.5.2 Gas-Source Doping

#### 3.5.3 Solid-Source Diffusion

### 3.6 Dopant Diffusion

- PN junction
- junction depth

$$
N(x,t)=\frac{N_0}{\sqrt{\pi D t}}\exp(-x/4Dt)
$$

$D$ is the **diffusivity**. 

**Shallow junctions** and **rapid thermal annealing**:

- furnace annealing
- rapid thermal annealing (RTA)
- rapid thermal oxidation (RTO)
- rapid thermal chemical vapor deposition (RTCVD)
- rapid thermal processing (RTP)
- flash annealing
- laser annealing
- transient enhanved diffusion (TED)

### 3.7 Thin-Film Deposition

- solid material
  - crastalline
  - polycrystalline
  - amorphous

#### 3.7.1 Sputtering

Spttering can be combined with a chemical reaction in **reactive sputtering**.

Sputtering is sometimes called a method of **physical vapor deposition (PVD)**.

#### 3.7.2 Chemical Vapor Deposition (CVD)

- step coverage
- high-temperature oxide (HTO)
- low-pressure chemical vapor deposition (LPCVD)
- plasma-enhanved chemical vapor deposition (PECVD)
- in situ doping

#### 3.7.3 Epitaxy

- hetero-junction

### 3.8 Interconnect—The Back-End Process

- metallization
- intermetal dielectric
- via
- electromigration
- damascene
- chemical-mechanical polishing (CMP)
- low-*k* dielectrics
- cross talk
- front-end process
- planarization

### 3.9 Testing, Assembly, and Qualification

- multi-chip modules (MCM)
- solder bumps
- flip-chip
- qualification
- operating life test
- burn-in


## 4. PN and Metal-Semiconductor Junctions

A PN junction has rectifying current-voltage characteristics, as a device, it is called a **rectifier** or a **diode**.

### 4.1 Building Blocks of the PN Junction Theory

The idealized PN juction has the uniformly doped P and N layers, known as **step junction** or **abrupt junction**.

#### 4.1.1 Energy Band Diagram and Depletion Layer of a PN Junction

#### 4.1.2 Built-In Potential

$$
\phi_{bi}=\frac{kT}q\ln\frac{N_dN_a}{n_i^2}
$$

Typically,$\phi_{bi}$ is about 0.9 V for a silicon PN junction.

#### 4.1.3 Poisson's Equation

$$
\frac{\mathrm d^2V}{\mathrm d x^2}=-\frac{\mathrm d E}{\text d x}=-\frac\rho{\varepsilon_S}
$$

$\varepsilon_S$ is the semiconductor permittivity and, for silicon, is equal to 12 times the permittivity of free space. $\rho$ is the charge density and $E$ is the electric field.

### 4.2 Depletion-Layer Model

The charge density is zero everywhere except in the depletion layer.

#### 4.2.1 Field and Potential in the Depletion Layer

> The depletion layer penetrates primarily into the lighter doping side, and the width of the depletion layer in the heavily doped material can often be neglected. It may be helpful to think that a heavily doped semiconductor is similar to metal.

$$
E(x)=\begin{cases}\frac{qN_a}{\varepsilon_S}(x_P-x)\quad 0\le x\le x_P\\ \frac{qN_d}{\varepsilon_S}(x-x_N)\quad x_N\le x\le 0\end{cases}
\\V(x)=\begin{cases}-\frac{qN_a}{2\varepsilon_S}(x_P-x)^2\quad 0\le x\le x_P\\ \phi_{bi}-\frac{qN_d}{2\varepsilon_S}(x-x_N)^2\quad x_N\le x\le 0\end{cases}
$$

#### 4.2.2 Depletion-Layer Width

$$
W_{dep}=x_P-x_N=\sqrt{\frac{2\varepsilon_S\phi_{bi}}q(\frac1{N_a}+\frac1{N_d})}
$$

The depletion-layer width is determined by the lighter doping concentration.

### 4.3 Reverse-Biased PN Junction

$$
W_{dep}=\sqrt{\frac{2\varepsilon_S(\phi_{bi}+V_r)}{qN}}
$$

> The depletion layer widen as the junction is more reverse biased to dissipate the extra voltage drop across it.

### 4.4 Capacitance-Voltage Characteristics

$$
C_{dep}=A\frac{\varepsilon_S}{W_{dep}}
$$

Numerically, $C\approx 1 f\text{F/}\mu m ^2$ when $W_{dep}=0.1\mu m$.

### 4.5 Junction Breakdown

There is nothing inherently destructive about junction breakdown. 

#### 4.5.1 Peak Electric Field

$$
E_p=E(0)=\sqrt{\frac{2qN}{\varepsilon_S}(\phi_{bi}+|V_r|)}\\
V_B=\frac{\varepsilon_SE_{crit}^2}{2qN}-\phi_{bi}
$$

#### 4.5.2 Tunneling Breakdown

$$
J=Ge^{-H/\varepsilon_p}
$$

$G$ and $H$ are constants for a given semiconductor.

#### 4.5.3 Avalanche Breakdown

$$
V_B=\frac{\varepsilon_SE_{crit}^2}{2qN}\approx15\times(\frac{10^{17}}{N})^{0.6}
$$

For silicon, $E_{crit}$ is about $5\times 10^5$ V/cm at $N=10^{17}\text{cm}^{-3}$,and is approximately proportional to $N^{0.2}$.

### 4.6 Carrier Injection Under Forward Bias—Quasi-Equilibrium Boundary Condition

$$
n(x_P)=n_{P0}e^{qV/kT}=\frac{n_i^2}{N_a}e^{qV/kT}\\
p(x_N)=p_{N0}e^{qV/kT}=\frac{n_i^2}{N_d}e^{qV/kT}
$$

This equation is called the **quasi-equilibrium boundary condition** or the **Shockley boundary condition**. $\exp(qV/kT)=10^{10}$ when forward bias is 0.6V. This equation is also valid for a reverse bias, in which situation the minority carrier is essentially zero, known as **minority carrier extraction**.
$$
\Delta n(x_P)=n(x_P)-n_{P0}=n_{P0}(e^{qV/kT}-1)\\
\Delta p(x_N)=p(x_N)-p_{n0}=p_{N0}(e^{qV/kT}-1)
$$

### 4.7 Current Continuity Equation

$$
\frac{\text d ^2\Delta p}{\text d x^2}=\frac{\Delta p}{D_p\tau_p}=\frac{\Delta p}{L_p^2}\\
\frac{\text d ^2\Delta n}{\text d x^2}=\frac{\Delta n}{D_n\tau_n}=\frac{\Delta n}{L_n^2}\\
$$

$L_n$ and $L_p$ are called the hole and electron **diffusion lengths**. They vary from a few $\mu m$ to hundreds of $\mu m$ depending on $\tau$.

### 4.8 Excess Carriers in Forward-Biased PN Junction

$$
\Delta p(x)=p_{N0}(e^{qV/kT}-1)e^{-(x-x_N)/L_p},\quad x>x_N\\
\Delta n(x)=n_{P0}(e^{qV/kT}-1)e^{(x-x_P)/L_n},\quad x< x_P
$$

The exponentially decaying density is because diffuse and recombination.

### 4.9 PN Diode IV Characteristics

$$
\text{Total current}=J_{pN}(x_N)+J_{nP}(x_P)=(q\frac{D_p}{L_p}p_{N0}+q\frac{D_n}{L_n}n_{P0})(e^{qV/kT}-1)\\
I=I_0(e^{qV/kT}-1)\\
I_0=Aqn_i^2(\frac{D_p}{L_pN_d}+\frac{D_n}{L_nN_a})
$$

$A$ is the diode area and $I_0$ is known as the **reverse saturation current**. It is often said that Si PN diodes have a turn-on voltage of about 0.6V at room temperature. 

#### 4.9.1 Contributions from the Depletion Region

We neglect hte recombination in the depletion region before. In reality, that contributes to the current, known as the **SCR current** for **space-charge region current**.
$$
pn=n_i^2e^{qV/kT}
$$
Recombination rate is the largest where
$$
n\approx p\approx n_ie^{qV/2kT}\\
\text{net recombination rate}=\frac{n_i}{\tau_{dep}}(e^{qV/2kT}-1)\\
I=I_0(e^{qV/kT}-1)+A\frac{qn_iW_{Dep}}{\tau_{dep}}(e^{qV/2kT}-1)\\
I_{\text{leakage}}=I_0+A\frac{qn_iW_{dep}}{\tau_{dep}}
$$

### 4.10 Charge Storage

$$
Q=I\tau_S
$$

$\tau_S$ is called the **charge-storage time**.

### 4.11 Small-Signal Model of the Diode

The diode appears to the analog circuit as a parrallel RC circuit.
$$
G=\frac1R=\frac{\text d I}{\text d V}=I_{DC}\bigg/\frac{kT}q\\
C=\frac{\text d Q}{\text d V}=\tau_S\frac{\text d I}{\text d V}=\tau_SG=\tau_SI_{DC}\bigg/\frac{kT}q
$$
$\tau_S$ is often called the **diffusion capacitance** or the **charge-storage capacitance**.

To be more accurate, one can add to the second equation a term $A\varepsilon_S/W_{dep}$, repsenting the depletion-layer capacitance. Under strong forward bias, the diffusion capacitance usually overwhelms it.

### 4.12 Solar cells

#### 4.12.1 Solar Cell Basics

$$
I=I_0(e^{qV/kT}-1)-I_{SC}
$$

$I_{SC}$ stands for **short-circuit current**, it is proportional to the light intensity and to the cell area.

#### 4.12.2 Light Penetration Depth—Direct-Gap and Indirect-Gap Semiconductors

$$
\text{Light intensity}(x)\propto e^{-\alpha x}
$$

$\alpha$ is called the **absorption coefficient**. $1/\alpha$ is called the light **penetration depth**.
$$
I_{sc}=AJ_p(0)=AqL_pG
$$

The open-circuit voltage:
$$
V_{oc}=\frac{kT}q\ln(\tau_pGN_d/n_i^2)
$$

#### 4.12.4 Output Power

$$
P=I_{sc}\times V_{oc}\times FF
$$

$FF$ is called the **fill factor**, which is the ratio of the maximum $|I\times V|$ to $I_{sc}\times V_{oc}$. $FF$ is typically around 0.75.

### 4.13 Light-Emitting Diodes and Solid-State Lighting

#### 4.13.1 LED Materials and Structures

#### 4.13.2 Solid-State Lighting

### 4.14 Diode Lasers

#### 4.14.1 Light Amplification

#### 4.14.2 Optical Feedback

#### 4.14.3 Diode Laser Applications

### 4.15 Photodiodes

### 4.16 Schottky Barriers

$$
\phi_{Bn}+\phi_{Bp}=E_g\\
\phi_{Bn}=\psi_M-\chi_{Si}
$$

- Fermi-level pinning

### 4.17 Thermionic Emission Theory

$$
v_{thx}=-\sqrt{2kT/\pi m_n}\\
J_{S\rightarrow M}=-\frac12 qnv_{thx}=\frac{4\pi qm_nk^2}{h^3}T^2e^{-q\phi_B/kT}e^{qV/kT}\\
=J_0e^{qV/kT}
$$

- $J_0\approx 100\exp(-q\phi_B/kT)$ is larger if $\phi_B$ is smaller
- $J_{S\rightarrow M}$ is only a function of $\phi_B-V$

### 4.18 Schottky Diodes

$$
I=I_0(e^{qV/kT}-1)\\
I_0=AKT^2e^{-q\phi_B/kT}
$$

$K\approx 100\text A/(\text{cm}^2/\text K^2)$ is known as the **Richardson constant**.

### 4.19 Applications of Schottky Diodes

### 4.20 Quantum Mechanical Tunneling

Tunneling probability
$$
P\approx \exp\left(-2T\sqrt{\frac{8\pi^2m}{h^2}(V_H-E)}\right)
$$

### 4.21 Ohmic Contacts

$$
T\approx W_{dep}/2=\sqrt{\frac{\varepsilon_S\phi_{Bn}}{2qN_d}}\\
P\approx e^{-H\phi_{Bn}/\sqrt{N_d}}\\
H=\frac{4\pi}{h}\sqrt{\frac{\varepsilon_S m_n}q}\\
J_{S\rightarrow M}=-J_{M\rightarrow S}=\frac12qN_dv_{thx}P
$$

If a small voltage is applied, the balance between $J_{S\rightarrow M}$ and $J_{M\rightarrow S}$ is broken.
$$
J_{S\rightarrow M}=\frac12qN_dv_{thx}e^{-H(\phi_{Bn}-V)/\sqrt{N_d}}\\
R_c=\frac VJ=\frac{2e^{H\phi_{Bn}/\sqrt{N_d}}}{qv_{thx}H\sqrt{N_d}}
$$
$R_c$ is the **specific contact resistance**.

## 5. MOS Capacitor

### 5.1 Flat-Band Condition and Flat-Band Voltage

$$
V_{fb}=\Psi_g-\Psi_s
$$

### 5.2 Surface Accumulation

$$
V_g=V_{fb}+\phi_s+V_{ox}\\
V_{ox}=\varepsilon_{ox}T_{ox} =-\frac {Q_{sub}}{C_{ox}}
$$

### 5.3 Surface Depletion

$$
V_{ox}=-\frac{Q_{sub}}{C_{ox}}=-\frac{Q_{dep}}{C_{ox}}=\frac{qN_aW_{dep}}{C_{ox}}=\frac{\sqrt{qN_a2\varepsilon_s\phi_s}}{C_{ox}}\\
V_g=V_{fb}+ \frac{qN_aW_{dep}^2}{2\varepsilon_s}+\frac{qN_aW_{dep}}{C_{ox}}
$$

### 5.4 Thershold Condition and Threshold Voltage

$$
\phi_{st}=2\phi_B=2\frac{kT}q\ln{\frac{N_a}{N_i}}\\
V_t=V_{fb}+2\phi_B+\frac{\sqrt{qN_a2\varepsilon_s2\phi_B}}{C_{ox}}
$$

### 5.5 Strong Inversion Beyond Threshold

$$
W_{dmax}=\sqrt{\frac{2\varepsilon_s2\phi_B}{qN_a}}\\
Q_{inv}=-C_{ox}(V_g-V_t)
$$

#### 5.5.1 Choice of $V_t$ and Gate Doping Type

$$
Q_{dep}=qN_aW_{dep}
$$

### 5.6 MOS C-V Characteristics

$$
C_{dep}=\frac{\varepsilon_s}{W_{dep}}\\
\frac1C=\frac1{C_{ox}}+\frac1 {C_{dep}}\\
\frac1C=\sqrt{\frac1{C_{ox}^2}+\frac{2(V_g-V_{fb})}{qN_a\varepsilon_s}}
$$

### 5.7 Oxide Charage—A Modification to $V_{fb}$ and $V_t^4$

$$
V_{fb}=V_{fb0}-\frac{Q_{ox}}{C_{ox}}
$$

### 5.8 Poly-Si Gate Depletion—Effective Increase in $T_{ox}$

$$
W_{dpoly}=\frac{\varepsilon_{ox}V_{ox}}{qN_{poly}}\\
C=\left(\frac1{C_{ox}}+\frac1{C_{poly}}\right)^{-1}=\left(\frac{T_{ox}}{\varepsilon_{ox}}+\frac{W_{dpoly}}{\varepsilon_s} \right)^{-1}=\frac{\varepsilon_{ox}}{T_{ox}+W_{dpoly}/3}\\
Q_{inv}=-C_{ox}(V_g-\phi_{poly}-V_t)
$$

### 5.9 Inversion and Accumulation Charge-Layer Thicknesses and Quantum Mechanical Effect

$$
T_{oxe}=T_{ox}+W_{dpoly}/3+T_{inv}/3\\
Q_{inv}=-C_{oxe}(V_g-V_t)=\frac{\varepsilon_{ox}}{T_{oxe}}(V_g-V_t)
$$

### 5.10 CCD Image and CMOS Imager

#### 5.10.1 CCD Imager

- Charge-coupled device
- Deep-depletion

#### 5.10.2 CMOS Imager

## 6. MOS Transistor

### 6.1 Introduction to the MOSFET

- source
- drain
- FET
- transistor

### 6.2 Complementary MOS (CMOS) Technology

### 6.3 Surface Mobilities and High-Mobility FETs

#### 6.3.1 Surface Mobilities

$$
I_{ds}=WQ_{inv}v=WQ_{inv}\nu_{ns}E \\=WC_{oxe}(V_{gs}-V_t)\mu_{ns}V_{ds}/L
$$

$W$ is the channel width, $E$ is the channel electric field, $\mu_{ns}$ is the electron **surface mobility** or the **effective mobility**.
$$
\frac{E_b+E_t}2=\frac{\varepsilon_{ox}}{2\varepsilon_sT_{oxe}}(V_{gs}+V_t+0.2\text V)\\
=\frac{V_{gs}+V_t+0.2\text V}{6T_{oxe}}\quad \text{for N}^+\text{ poly-gate NFET}
$$

#### 6.3.2 GaAs MESFET

Use a Schottky junction to serve as the control gate of a FET, called MESFET for metal-semiconductor field-effect transistor.

- If the transistor is conductie at $V_g=0$ and requires a reverse bias gate voltage to turn it off, it is called a **depletion-mode transistor**.
- If a forward gate voltage is needed to turn the transistor on, this is known as an **enhancement-mode transistor**.

#### 6.3.3 HEMT

By growing a thin epitaxial layer of GaAlAs over the undoped GaAs substrate, we significantly increased the electron mobility. This device is called **HEMT** or **high electron-mobility transistor**, or **MODFET** for **modulation- doped FET**. It is used in microwave communication, satellite TV receivers, etc.

#### 6.3.4 JFET

If the Schottky junction in MESFET is replaced with a $\text P ^+\text N$ junction, the new structure is called a **JFET** or **junction field-effect transistor**.

### 6.4 MOSFET $V_t$, Body Effect, and Steep Retrograde Doping

$$
V_t(V_{sb})=V_{t0}+\frac{C_{dep}}{C_{oxe}}V_{sb}=V_{t0}+\alpha V_{sb}
$$

The fact that $V_t$ is a function of the body is called the **body effect**. $\alpha$ is called the **body effect coefficient**.

**Steep retrograde body doping profiles**: light doping in a thin surface layer and very heavy doping underneath.

### 6.5 $Q_{inv}$ in MOSFET

$$
Q_{inv}(x)=-C_{oxe}(V_{gs}-mV_{cs}-V_t)\\
m=1+\alpha =1+C_{dep}/C_{oxe}=1+3T_{oxe}/W_{dmax}
$$

The body is sometimes called the **back gate** since it clearly has a similar though weaker effect on the channel charge. The back-gate effect on $Q_{inv}$ is often called the **bulk-charge effect**. $m$ is called the **bulk-charge factor**.

### 6.6 Basic MOSFET IV Model

$$
I_{ds}=\frac W LC_{oxe}\mu_{ns}(V_{gs}-V_t-\frac m2V_{ds})V_{ds}\\
V_{dsat}=\frac{V_{gs}-V_t}m
$$

$V_{dsat}$ is called the **drain saturation voltage**, 

### 6.7 CMOS Inverter--A Circuit Example

#### 6.7.1 Voltage Transfer Curve (VTC)

#### 6.7.2 Inverter Speed--The Importanvce of $I_{on}$

#### 6.7.3 Power Consumption

$$
P_{\text{dynamic}}=V_{dd}\times\text{average current}=kCV_{dd}^2f
$$

$f$ is the clock frequency and $k$ is an **activity factor** that represents the fact that a particular gate in a given circuit is not switched every clock cycle all the time.

> This dynamic power dominates the power consumption when the inverter is switched frequently. Power consumption can be reduced by lowering $V_{dd}$ and by minimizing all capacitances in the circuit as well as by reducing $k$. It is interesting to note that making $I_{on}$ large by using a small $L$ or improving the carrier mobility does not increase $P_{\text{dynamic}}$.

$$
P_{\text{static}}=V_{dd}I_{off}
$$

### 6.8 Velocity Saturation

### 6.9 MOSFET IV Model With Velocity Saturation

#### 6.9.1 Celocity Saturation vs. Pinch-Off

### 6.10 Parasitic Source-Drain Resistance

### 6.11 Extraction of the Series Resistance and the Effective Channel Length

### 6.12 Velocity Overshoot and Source Velocity Limit

### 6.13 Output Conductance

### 6.14 High-Frequency Performance

### 6.15 MOSFET Noises

#### 6.15.1 Thermal Noise of a Resistor

#### 6.15.2 MOSFET Thermal Noise

#### 6.15.3 MOSFET Flicker Noise

#### 6.15.4 Signal to Noise Ratio, Noise Factor, Noise Figure

### 6.16 SRAM, DRAM, Noncolatile (Flash) Memory Devices

#### 6.16.1 SRAM

#### 6.16.2 DRAM

#### 6.16.3 Nonvolatile (Flash) Memory

## 7. MOSFETs in ICs--Scaling, Leakage, and Other Topics

### 7.1 Thechnology Scaling--For Cost, Speed, and Power Consumption

#### 7.1.1 Innovations Enable Scaling

#### 7.1.2 Strained Silicon and Other Innovations

| Year                 | 2003             | 2005 | 2007            | 2010            | 2013   |
| -------------------- | ---------------- | ---- | --------------- | --------------- | ------ |
| Technology Node (nm) | 90               | 65   | 45              | 32              | 22     |
| Innovations          | Strained Silicon |      | High-k material | Wet lithography | FinFET |

### 7.2 Subthreshold Current--"Off" is Not Totally "Off"

$$
I_{ds}(nA)=100\cdot \frac WL\cdot e^{q(V_{gs}-V_t)/\eta kT}
$$

### 7.3 $V_t$ Roll-Off--Short-Channel MOSFETs Leak More

$$
V_t = V_{t-long}-(V_{ds}+0.4\text V)\cdot e^{-L/l_d}\\
l_d\propto\sqrt[3]{T_{oxe}W_{dep}X_j}
$$

### 7.4 Reducing Gate-Insulator Electrical Thickness and Tunneling Leakage

### 7.5 How to Reduce $W_{dep}$

### 7.6 Shallow Junction and Metal Source/Drain MOSFET

#### 7.6.1 MOSFET with Metal Source/Drain

### 7.7 Trade-Off Between $I_{on}$ and $I_{off}$ and Design for Manufacturing

### 7.8 Ultra-Thin-Body SOI and Multigate MOSFETs

#### 7.8.1 Ultra-Thin-Body MOSFET and SOI

#### 7.8.2 FinFET - Multigate MOSFET

### 7.9 Output Conductance

### 7.10 Device and Process Simulation

### 7.11 MOSFET Compact Model for Circuit Simulation

## 8. Bipolar Transistor

### 8.1 Introduction to the BJT

### 8.2 Collector Current

#### 8.2.1 High-Level Injection Effect

### 8.3 Base Current

### 8.4 Current Gain

#### 8.4.1 Emitter Band Gap Narrowing

#### 8.4.2 Narrow Band-Gap Base and Heterojunction BJT

#### 8.4.3 Poly-Silicon Emitter

#### 8.4.4 Gummel Plot and $\beta_F$ Fall-Off at High and Low $I_C$

### 8.5 Base-Width Modulation by Collector Voltage

### 8.6 Ebers-Moll Model

### 8.7 Transit Time and Charge Storage

#### 8.7.1 Base Charge Storage and Base Transit Time

### 8.7.2 Drift Transistor-Built-In Base Field

### 8.7.3 Emitter-to-Collector Transit Time and Kirk Effect

### 8.8 Small-Signal Model

### 8.9 Cutoff Freqency

### 8.10 Charge Control Model

### 8.11 Model for Large-Signal Circult Simulation

