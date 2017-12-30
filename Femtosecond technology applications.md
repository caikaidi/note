# Femtosecond technology applications

飞秒激光应用技术

**Hui Sun** sunhuisunhui@hotmail.com 13717662509

1. 飞秒激光医学应用
   - LASIK
   - 白内障
   - 激光和组织相互作用
   - 牙科
   - 神经外科
   - 耳科
2. 飞秒激光工业应用
   - 表面结构化
   - 金属打孔
   - 钻石切割
   - 度量衡

***教材***

《Femtosecond laser assisted LASIK eye surgery and imaging》Hui Sun, SPIE press, 2015

《OCT assisted Femtosecond laser cataract surgery》Hui Sun, SPIE press, 2017

《Femtosecond technology for technical and medical application》Friedrich dausinger, friedemann lichtner, Holger lubatschowski, Springer, 2004

***参考书***

《Laser tissue interactions: fundamentals and applications》Markolf H niemz, Springer, 2007

《Ultrashort laser pulses in biology and medicine》Markus Braun, Peter Gilch, Wolfgang Zinth, Springer, 2007

《Physics of laser materials processing》Gennody G Gladosh, Igor Smdnv, Springer, 2011

-----

@9.11

## 1. Laser

**Wavefront:** in physics, a wavefront is the locus of point characterized by propagation of positions of identical phase

Microscope -> telescope -> ophthalmology(1978)

Adaptive optics (AO)

Shack-Hartmann wavefront sensor

principle of AO:

- the first step: measuring an incoming wavefront by a wavefront sensor
- the second step: correcting the deformations of an incoming wavefront by deforming a mirror

Three types of aberration measurement devices:

1. The thin-beam ray-tracing aberrometer
2. The Tscherning aberrometer
3. Shark-Hartmann method

the laser

> **A laser** is a device that generates or amplifies coherent radiation at frequencies in the infrared, visible, or ultraviolet regions of the electromagnetic spectrum, then emits light through a process of optical amplification based on the stimulated emission of eletromagnetic radiation.

Essential elements of a laser:

- a laser medium
- a pumping process
- Suitable optical feedback elements

Pumping can be *a eletrical current* or *a light at a different wavelength*

Femtosecond  $10^-15 s$

**femtosecond laser** is a laser in which the pulse duration is in femtosecond range

Nd: glass	 Nd: YAG

Solid-state laser 	typically optically pumped: a glass lamp or laser diodes

a femtosecond laser has a few basic elements :

- a broadband gain medium
- a laser cavity
- an output coupler
- a dispersie element
- a phase modulator
- a gain/loss process controlled by the pulse intensity or energy

Laser tissue interactions

Structure of the cornea

Cornea accounts for two-thirds of the total refractive power

*smoothness of the corneal surface* & *total thickness of the cornea* lead to visual distortion

11 to 12mm horizontally and 9 to 11mm vertically and 0.5mm thick at the center

the optical properties of the cornea are determined by its transparency, surface smoothness,  contour, refractive index

Epithelium, Bowman's layer, storma(90%), Descement's membrane, endothelium

-----

@9.18

#### 1.3.2 physical principles of laser tissue interactions

a common finding is that the short pulse damage is deterministic in nature and the threshold is lower with shorter laser pulses

Laser tissue interactions: 

- Photochemical interactions
- thermal interactions
- Photo ablation
- Plasma induced ablation (femtosecond laser flap)(also called plasma mediated ablation)
- Photo disruption

a single parameter distinguishes and primarily controls these process: the duration of laser exposure

Laser induced optical breakdown (LIOB) $$10^{11} W/cm^2$$ in solids or fluids $$10^{14} W/cm^2$$ in air
$$
I(r,z,t)=\frac{1}{2}\varepsilon_0CE^2
$$
Q switched pulses: nanosecond

- First step
  - first you get the *thermionic emission*
  - from this one we get the *multiphoton ionization*
  - Both two above get a few elections initiate on avalanche effect
  - leading to the accumulation of free electrons
- second step
  - Accelerated electron absorbs a photon and accelerates: two free electrons
- third step
  - the two free electrons absorb accelerate two more
  - This step continued so more and more electrions were produced

Mode locked pulses: picosecond or femtosecond

a common finding: laser intensity is inversely proportional to laser pulse duration, namely laser breakdown thresholds decrease by the square root of the pulse duration over loofs to 100 ms

an optimal pulse duration for femtosecond laser corneal surgery in the few hundreds of femtosecond pulse duration ranges

## 2. LASIK surgery

### 2.1 LASIK procedure

LASIK is laser in situ keratomileusis.

as of 2011 over 11 million LASIK in US, 1million every year in US.

as of 2009 over 28 million in the whole world.

LASIK procedure consist two steps:

- a thin flap is created on the anterior surface of the cornea and lifted
- The underlying corneal stroma is ablated and then the flap is replaced

the layers of tissue removed are tens of micrometers thick

### 2.2 All solid state chirped pulse amplification(CPA) femtosecond laser

fs -> ps -> amplify -> fs

1. stretched out in time prior to introducing it to the amplifier
   - the low frequency component of the laser pulse travels a shorter path than the high high frequency component does, which is called group velocity dispersion(GVD).
2. Amplify
3. Recompressed back

GVD: prisms, or gratings, or GTI mirrors

laser come out from the fs laser oscillator: 76MHz  1nJ  <200fs

after CPA: 1KHz  5uJ  800fs

### 2.3 femtosecond laser assisted flap creation

before we use femtosecond laser, we use *microkeratome*: blade guality gap width of the microkeratome head, translation speed affert guality of the flap

advantages of femtosecond laser:

- primarly due to the enhanced precision and minimized collateral tissue effects.
- Greater accuracy in flap size, shape and thickness.

IntraLASIK and femtoLASIK are all laserLASIK

-----

@9.25

### 2.4 Commercially available femtosecond laser in refractive surgery

Intralase 2001	CPA

20/10 perfect vision 2001	CPA

Ziemer 2005

ziess 2006	CPA

Alcon 2010(wavelight) 2012(lenSx)	CPA

two groups:

1. High pulse energy $$\mu J$$ low frequency $$KHz$$
2. Low pulse energy $$nJ$$ high frequency $$MHz$$

## 3. safety study

50%~60% of enegy go through the cornea

(600fs 1053nm 150KHz)

The thermal camera is Ti55 Fluke camera

San Diego eye bank

1. Refractive index 1.33
2. 17mm

Now we talk about the simulation,

Assumptions:

- Four layer(neuro-sensory retina, RPE, choroid, sclera)

- average refractive index 1.33

- The high concentration of melanin pigments in retina is the main factor for absorption of laser energy 

- Upper: heat flux   Others: temperature 20$$^\circ C$$
  $$
  K\nabla T = h(T_{inf}-T)
  $$

- iris is big

- no heat flow due to blood flow

Heat diffusion equation
$$
\rho C_p\frac{\partial T}{\partial t}+\nabla\times(-k\nabla T)=Q\\
\begin{align}
&\rho - \text{Density}\qquad C_p-\text{Heat capacity}\\
&k-\text{Thermal conductivity}
\end{align}
$$

-----

@10.9

> 查一篇文献
>
> - 2017/2016
> - Femtosecond laser LASIK
> - pdf
> - 写一段文献内容
>
> yulongliuucas@sina.com

### 3.2 iris safety

Iris model

basic assumptions:

- one isotropic layer(iris pigment epithelium)

- an average refractive index 1.33

- the high concentration of melanin pigments in the iris is the main factor for absorption

- upper: heat flux    other: temperature
  $$
  k\nabla h =h(T_{inf}-T)
  $$

- the calculation of the heat absorbed by this iris was based on the Beer-Lambert law
  $$
  I=I_0e^{-\circ}
  $$










mathematical model

heat duffusion equation
$$
\rho C_p\frac{\partial T}{\partial t}+\nabla\times(-k\nabla T)=Q\\
\begin{align}
&\rho - \text{Density}\qquad C_p-\text{Heat capacity}\quad 3997\\
&k-\text{Thermal conductivity}\qquad Q-\text{enegy}
\end{align}
$$

## 4. Imaging technology for LASIK surgery

Two-photon microscope

Advantage:

- does not need an extra pinhole to get diffraction limited resolution and depth discrimination
- the two-photon microscope greatly reduces photo damage or a bleaching effect outside the laser focus


-----

@10.16

# OCT assisted femtosecond laser cataract sugery

## 1. cataracts and sugery

### 1.1 lens structure

the lens accounts for one-third of the total refractive power

a slight change in the lenticular contour, transparency, the shape of the lens: cause visual distortion 

Adult lens: 10mm in diameter   axial length of about 4mm

the lens has three main parts:

- capsule
- epithelial
- fibers

Reflect ration 1.306-1.468

# 1.2 cataracts

Either clumps of protein or yellow brown pigment maybe deposited in the lens, reducing the transmission of light to the retina, such opacity of the lens, whether it is a small local opcity or a diffuse general loss of transparency is called cataracts.

Signs of cataracts:

- faded colors
- blurry vision
- halos around lights
- trouble with bright lights
- trouble seeing at night

Three common types of cataracts:

- nuclear
- cortical
- Posterior sub-capsular

Grading systems:

- the Oxford clinical cataract classification and grading system
- the Johns Hopkins system
- the lens opacity classification system(LOSC I, LOCS II, LOCS III)

### 1.3 surgery

the standard of care in cataract surgery is removal of the cataract by two types of surgical procedures:

- Phaco emulsification(PE or phaco)
- Extracapsular cataract extraction 

following surgical remove of the crystalline lens, an artificial intraocular lens(IOL) is implanted.

PE or phaco is the most common technique today.

Surgical procedure in PE:

1. anesthetic: the eye is numbed by an injection
2. corneal incision: two cuts are made at the clear corneal
3. capsulorhexis: a small pair of forceps or a needle employed to create a circular hole in the capsule
4. PE or phaco: a handheld probe is used to emulsify the cataract and the lens parts are removed with suction. The irrigation and aspiration procedure is a succeeding step.
5. Lens insertion: the IOL is inserted into the capsular bag that formerly contained the crystalline lens
6. wound sealing: salt water in injected

### 2.3 laser tissue interactions

a common finding notes that the short pulse damage is deterministic in nature and that the threshold is lower with shorter laser pulses

CW 1s — photochemical interaction

1s< t < 1us — thermal interaction

1us< t < 1ns — photoablation

< 1ns — plasma induced ablation and photodisruption

#### 2.3.1 photochemical interaction

photochemical interactions take place at very low power densities, for example, 1 $w/cm^2$ and long exposure times range from seconds to a CW.

#### 2.3.2 thermal interaction

coagulation, vaporization, varbonization, melting

####2.3.3 photoablation

two advantages:

- the precision of the etching process
- The lack of thermal damage to adjacent tissues

#### 2.3.4 plasma induced ablation

LIOB $10^{11} w/cm^2$ in solid and fluid $10^{14} w/cm^2$ air without thermal or mechanical damage, the tissue is well defined and can be removed very clearly. Also called plasma mediated ablation.
$$
I(r,z,t)=\frac 1 2 \varepsilon_0 CE^2
$$

#### 2.3.5 photodisruption

**Plasma formation** and **shock-wave generation** are physical effects associated with optical breakdown **cavitation** and **jet formation** may additionally take place if breakdown occurs inside soft tissues or fluids.

Different than the plasma induced ablation, the secondary effects of plasma at higher pulse energies (such as shock waves) become more significant.

In the breakdown region, the effect is plasma induced ablation, while in the adjacent region the effects are shock waves and cavitation.

-----

@10.23

The difference between the plasma induced ablation and photodisruption is the different power enegy during the process.

Shock wave generation and cavitation are the primary mechanisms, completed by jet formation if the cavitation's collapse is in fluids and near a solid boundary.

Plasma formation, shock wave generation, cavitation and jet formation occur on different time scales.

Laser breakdown thresholds decrease by the square root of the pulse duration over the 100fs to 100us range.

### 2.4 Optical coherence tomography in ophthalmic application

Hardware: Michelso interferometer

Like in a Michelson interferometer, light in an OCT system is split into two arms — a sample arm and a reference arm. When the light from both of the arms has traveled an optical distance that is a difference of less than a coherent length, the combination of reflected light from the sample arm and reference light from the reference arm produces an interferenve pattern.

This reflectivity profile, called an A-scan, contains information about the spatial dimensions and locations of structure within the item of interest. A cross-sectional tomography, called a B-scan, may be achieved by laterally combing a series of A-scans.

An OCT system for which the path length of the reference arm is translated longitudinally in time is called a time-domain OCT.

An OCT system for which the broadband interference is acquired with spectrally separated detectors is called a frequency-domain OCT. IT is also called a Fourier-domain OCT (FD-OCT). 

Use of OCT:

- anterior segment imaging
- retina imaging

## 3. OCT-guided femtosecond laser cataract surgery

### 3.1 commercially available femtosecond lasers

LASIC: Intralase, 20/10 perfect vision, Zeiss, Ziemer, Alcan(wave light, lenSx)

Catarat: catalys, victus, , Femto LDV, LenSx, LensAR

> - Femtosecond cataract 
> - 2017/2016
> - 写内容 word 100-200

-----

@10.30

#### 3.1.1 lenSx

#### 3.1.2 Catalys

#### 3.1.3 lensAR Scheimpflug chamber

#### 3.1.4 Victus

#### 3.1.5 Femto LDV

### 3.2 surgery procedures

femtosecond laser assisted cataract surgery(FLACS)

Several aspects of contaract surgery, such as the clear corneal incisions, creation of the capsulotomy, fragmentation of the lens nucleus, and correction of astigmatism through corresponding arcuate incision, may currently be assisted or replaced by femtosecond lasers.

four steps:

- planning
- engagement
- Visualization and customization
- treatment

#### 3.2.1 planning

The planning parameters include: 

- Location, depth, and architecture of incisions for corneal incisions
- Size, shape, and desired center of laser ablation for capsulotomy
- Diameter, depth, and patterns of cut for lens fragmentation

#### 3.2.2 engagement

The patient interface optically couples the eye to the optical delivery system to prevent eye movement.

This is the first clinical step for FLACS. The docking system, namely the patient interface, is normally composed of a curved application lens and suction ring.

An ideal patient interface should satisfy three requirements:

- It should fix the eye without distorting the eye and causing the intraocular pressure(IOP) to increase
- It should have a wide field of view to allow for surgical facility
- It should have the ability to prevent corneal folds that occur with suction, and allow for a tight laser focus

#### 3.2.3 visualization and customization

The image guidance sub-system gives the interaction about the dimensions and location of ocular structures. It guides the surgeon through lens fragmentation zones and the placement of incisions.

#### 3.2.3 treatment

The treatment includes four parts: clear cormeal incisions, creation of the capsulotomy, fragmentation of the lens nucleus, and correction of astigmatism through corresponding arcuate incisions.

After the application of a femtosecond laser, a standard manual PE or phaco will be used to remove the broken crystalline lens. After the removal of the cataract, an IOL is usually implanted into the eye.

-----

@11.6

### 3.3 Benefits

FLACS advantages: 

- a better quality of incision with reduced induced astigmatism 
- increased reliability and reproducibility of the capsulotomy with increased stability of the implanted lens
- a reduction in the use of ultrasound

#### 3.3.1 corneal incision

One of the most important advantage of FLACS is that the corneal incisions can be designed to construct reproducible and stable incisions, so that the incision width and length may be customized according to this precept with a high degree of integrity.

Corneal wounds and arcuate incisions in the desired position and depth make the control of postoperative astigmatism much more effective.

#### 3.3.2 capsulotomy

If FLACS can produce a reproducibly round, centered, and intact anterior capsule, this along would improve the safety of cataract surgery in a way that could possible justify the introduction of this new technology.

FLACS can produce a more precise, reproducible, better centered, and stronger opening of the anterior capsule than conventional manual continuous curvilinear capsulorhexis(CCC).

$\rightarrow$permits for a better IOL and capsule overlap

#### 3.3.3 lens fragmentation

Femtosecond laser cuts on the crystalline lens soften the harder cataracts and decrease in the amount of ultrasound energy from the PE probe, thereby diminishing the risk of capsule complications and corneal endothelial injury.

#### 3.3.4 other benefits

Other benefits of FLACS include the ability to correct astigmatism through corresponding arcuate incisions, a reduction of infection possibility, decreased endothelial cell loss, and possible improved visual and refractive outcomes.

### 3.4 safety

ANSI 21361-2007

# laser tissue interaction

### 3.0 interaction mechanisms

coefficients of reflection, absorption and scattering

this three things determine the total transmission of the tissue at a certain wavelength.

Parameters are given by the laser:

- wavelength
- Exposure time
- Applied energy
- focal spot size
- energy density
- Power density

### 3.1 photochemical interaction

The group of photochemical interactions stems from empirical observations that light can introduce chemical effects and reactions with macromolecules or tissues.

Photochemical interaction mechanisms play a significant role during photodynamic therapy(PDT).

Photochemical interactions take place at very low power densities (typically 1$w/cm^2$) and long exposure times ranging from seconds to continuous wave.

During PDT, spectrally adopted chromophores are injected into the body. Monochromatic invadiatino may then trigger selective photochemical reactions, resulting in certain biological transformations.

The main idea of photochemical treatment is to use a chromophore receptor acting as a catalyst.

This also called photosensitized oxidation.

After the absorption of laser photons, the photosensitizer is first transferred to an excited singlet state $^1S^*$, then three potential decay channels are available: nonratiative and radiative singlet decay to the singlet fround state, and intersystem crossing to an excited triplet state.

The radiative singlet and triplet decays are called fluorescence and phosphorescence, respectively. 

Typical lifetimes of fluorescence are of the order of nanoseconds, whereas phosphorescence may last up to a few milliseconds or seconds.

#### 3.1.1 photodynamic therapy(PDT)

PDT is performed as follows:

Injection -> clearance -> irradiation -> transfer reactions -> necrosis

First, a photosensitizer eg. HpD, is inject into a vein of the patient, within the next few hours, HpD is distributed among all soft tissues except the brain.Then the basic characteristic of a photosensitizer is that it remains inactive untill irradiated. After 48-72 hours, most of it is cleared from healthy tissue. Its concentration in tumor cells has not decreased much even after a period of 7-10 days.

-----

@11.13

Laser irradiation usually takes place after the third day and up to the seventh day after injection if several treatment are necessary. Within this period, tumor cells are still very sensitive and selective necrosis of tumor cells is enabled.

dihematoporphyrin(HpD)

The simultaneous diagnosis and therapy of tumors with photosensitizers is one of the key advantages of PDT.

The major disadvantage of HpD is the fact that hte patient needs to remain in a dark room during the first weeks of therapy.

#### 3.1.2 biostimulation

Biostimulation is believed to occur at very low irradiances and to belong to the group of photochemical interactions.

The potential effects of extremely low laser power(1-5mw) on biological tissue have been a subject of controversy.

#### 3.1.3 summary of photochemical interaction

main idea: using a photosensitizer acting as catalyst(only in photodynamic therapy)

Observations: no macroscopic observations

typical lasers: red dye laser, diode lasers

typical pulse durations: 1s — CW(continue wavelight)

typical power densities: 0.01 — 50 $w/cm^2$

special applications: photodynamic therapy, biostimulation

### 3.2 thermal interaction 

The term thermal interaction stands for a large group of interaction types, where the increase in local temperature is the significant paraneter change. Thermal effects can be induced by either CW or pulsed laser radiation. 

Different effects: coagulation, vaporization, carbonization, melting

The reaction with a target molecule $A$ can be considered as a two step process first, absorption of a photon with an energy $h\nu$ promotes the molecule to an excited state $A^*$, second inelastic collisions with some partner $M$ of the surrounding medium lead to a deactivation of $A^*$ and a simultaneous increase in the kinetic enegy of $M$.

Therefore, the temperature rise microscopically originates from the transfer of photon enegy to kinetic enegy.
$$
\begin{align}
&\text{absorption:}\quad A + h\nu \rightarrow A^*\\
&\text{deactivation:}\quad A^* + M(E_{kin})\rightarrow A +M(E_{kin}+\Delta E_{kin})
\end{align}
$$
For the description of storage and transfer of heat, thermal tissue properites are of pirmary importance such as heat capacity and thermal conductivity.

-----

@11.20

Heat generation is determined by laser parameters and cptical tissue properties — primarily irradiance, exposuvretime, and absorption coefficient — with the absorption coefficient itself being a function of the laser wavelength.

Heat transport is solely characterized by thermal tissue properties such as heat conductivity and heat capacity. Heat effects, finally, depend on the type of tissue and temperature achieved inside the tissue.
$$
\vec E (r,z,t)= \vec E_0 \exp(-\frac{r^2}{w^2}-\frac{\alpha z}{2})\exp(-\frac{4t^2}{\tau^2})\\
\vec I (r,z,t)= I_0 \exp(-\frac{2r^2}{w^2}-\alpha z)\exp(-\frac{8t^2}{\tau^2})\\
w: \text{beam wuist}\quad \alpha: \text{absorption coeffcient}\quad \tau: \text{palse duration}\\
r=w \quad \tau=t/2 \quad I=\frac{1}{e^2}I_0\quad I_0=\varepsilon_0c\vec {E_0^2}/2
$$

#### 3.2.1 heat generation

$$
S(r,z,t)=\frac{I(r,z,t)-I(r,z+\Delta z,t)}{\Delta z}\qquad \frac{W}{cm^2}\\
\text{when}\Delta z\rightarrow0,\quad S(r,z,t)=-\frac{\partial I(r,z,t)}{\partial z}\\
\text{heat deposition:}\quad S(r,z,t)=\alpha I(r,z,t)\\
$$

$$
\mathrm d Q =mc\cdot\mathrm d T\\
\text{m: tissue mass}\quad \text{c: heat capacity} KJ\cdot kg^{-1}\cdot K^{-1}\\
c=(1.55+2.8\frac{\rho_w}{\rho})\quad \rho:\text{tissue dencity}\quad \rho_w:\text{water contant}\\
$$

#### 3.2.2 heat transport 

$$
\vec {j_Q}=-K\nabla T\quad K:\text{heat conductivity}\quad w\cdot m^{-1}\cdot K^{-1}\\
K=(0.06+0.57\frac{\rho_w}{\rho})\quad K=0.63 \quad T=37^\circ C\\
k=\frac{K}{\rho c}\quad \frac{m^2}{S}\quad \text{temperature conductivity}\\
$$

Temperature change in heat content per unit volume $\dot q$
$$
\mathrm{div} \vec{j_Q}= -\dot q\\
\mathrm d Q=mc\cdot \mathrm d T\\
\dot T = \frac{1}{mc}\dot Q= \frac{1}{\rho c}\frac{\dot Q}{V}= -\frac{1}{\rho c}\mathrm{div}\vec{j_Q}\\
\dot T=k\Delta T\quad \text{homogeneous heat conduction equation}\\
\dot T = - \frac{1}{\rho c}(\mathrm{div}\vec{j_Q}-S)\\
\dot T = k\Delta T+\frac{1}{\rho c}S\\
Z_{therm}(t)=\sqrt{4kt}\\
L=\sqrt{4k\tau_{therm}}
$$
$\tau_{therm}$: thermal relaxation time 

For laser pulse duration $\tau<\tau_{therm}$, heat does not even diffuse to the distonce given by the optical penetration depth $L$. Hence, thermal damage of nondecomposed tissue is negligible. 

For $\tau>\tau_{therm}$, heat can diffuse to a multiple of the optical penetration depth, ie, thermal damage of tissue adjacent to the decomposed volume is possible.

Laser palse duration $\tau<1 \mu s$ are usually not associated with thermal damage this statement is also refered to as the "1$\mu s $ rule"

- Case I: $\tau < 1\mu s$ for nanosecond or picosecond pulses, heat diffusion during the laser pulse is negligible.

$$
S = \alpha I_0\\
T = \begin{cases} T_0+\frac{\alpha I_0}{\rho C}t \quad 0\leq t<\tau\\
T_0 + T_{max}(\frac{\tau}{t})^{2/3}\quad t>\tau
\end{cases}\\
T_{max}= \frac{\alpha I_0}{\rho c}\tau\quad \text{at }t=\tau\\
$$

- Case II: $\tau>1\mu s$ for pulse duration during which heat diffusion is considerable, the thermally damaged zone is significantly broadened.

  A high repetition rate $\nu_{rep}$ of the laser pulses can evoke an additional increase in temperature if the rate of heat transport is less than the rate of heat generation.

We assume a pulse energy of 3$\mu J$ is absorbed within a tissue volume of 1000 $\mu m ^3$ which contams 80% water.

We know: the amount of water in the specified volume is $8\times 10^{-10}g$.

1. Laser energy is needed to heat the tissue up to 100$^\circ C$ 
2. Energy is transferred to vaporization teat
3. the remaining energy leads to a further increase in temperature of the water vapor.



1. $37 ^\circ C\rightarrow 100^\circ C$

   $Q_1 = mc\Delta T = 8\times10^{-10}\times43\times 63 = 2.2\times 10^{-7}J$

2. Vaporization at 100$^\circ C$

   $Q_2 = mQ_{vap}=8\times 10^{-10}\times 2253 = 1.8\times 10^{-6}J$

3. $100^\circ C\rightarrow T_{tin}$

   $Q_3= 3-Q_1-Q_2=0.98\mu J$

   $T_{tin}=100+\frac{Q_3}{mc}=100+\frac{0.98}{8\times 10^{-10}\times 43}\approx 385^\circ C$

-----

@11.27

#### 3.2.3 heat effects

Thermal effects of laser radiation

Body 37$^\circ C$ no measurable effects for the next 5$^\circ C$

|  temperatrue   | biological effect                        |
| :------------: | :--------------------------------------- |
|  37$^\circ C$  | normal                                   |
|  45$^\circ C$  | Hyperthermia                             |
|  50$^\circ C$  | Reduction in enzyme activity, cell immobility |
|  60$^\circ C$  | Denaturation of proteins and collagen, coagulation |
|  80$^\circ C$  | Permeabilization of membranes            |
| 100$^\circ C$  | vaporization, thermal decomposition(ablation) |
| $>100^\circ C$ | Carbonization                            |
| $>300^\circ C$ | Melting                                  |

As a matter of fact, it was observed that not only the temperature achieved but also the temporal duration of this temperature plays a significant roll for the induction of irreversible damage.

*Arrhenius's equation:*
$$
\ln\frac{C(t)}{C_0}= -A\int_0^t\exp(-\frac{\Delta E}{RT(t^\prime)})\mathrm d t^\prime \equiv-\Omega\\
C_0:\text{initial concentration of molecules or cells}\\
C(t):\text{concentration at time }t\\
A:\text{Arrhenius' constant}\quad R: \text{universial gas constant}\\
\Delta E \&\Omega: \text{specific tissue propoties}\\
A\approx\frac{KT}{h}\exp\frac{\Delta S}{R}\\
\Delta S: \text{activation entropy}\quad K:\text{Boltzmann's constant}\\h:\text{Planck's constant}\\
D_{d(t)}=\frac{c_0-c_t}{c_0}=1-\exp(-\Omega)
$$
Laser radiation acts thermally if power densities $\ge 10 w/cm^2$ and applied from either CW radiation or pulse duration exceeding approximetely $1 \mu s$. Typical lasers for coagulation are Nd:YAG lasers or diode lasers.

$CO_2$ lasers are very suitable for vaporizatino and the precise themal cutting of tissue. Carbonization and melting can occur with almost any type of laser if sufficient power densities and exposure durations are provided.

<u>Melting, carbonization, vaporization, coagulation:x irreversible</u>

<u>Hyperthermia: reversible, irreversible</u>

<u>Exposure energy, exposure volume, exposure duration together determine the degree and extent of tissue damage.</u>

#### 3.2.4 laser induced interstitial themotherapy(LITT)

The possibility of localized coagulation has formed the basis of a novel tumor treatment called LITT.

The principle idea of LITT is to position and appropriate laser applicator inside the tissue to be coagulated, eg. a tumor, and to achieve necrosis by heating cells above 60$^\circ C$.

Since the optical penetration depth of laser light in the near infrared is very high, deeper zones are reached more easily by the machanism of light scattering rather than by heat conduction. Therefore, laser applications emitting radiation through a scattering surface are favored compared to focusing optics.

#### 3.2.5 summary of thermal interaction 

Main idea: achieving a certain temperature which leads to the desired thermal effect

Observation: either coagulation, vaporization, carbonization or melting

Typical lasers: $CO_2$, Nd:YAG, Er:YAG, Ho:YAG, argon ion and diode lasers.

Typical pulse durations: 1$\mu s $ —1min

Typical power densities:10 — $10^6 w/cm^2$

Special applications: coagulation, vaporization, melting, thermal decomposition, treatment of retinal detachment, LITT

### 3.3 photoablation

The removal of tissue was performed in a very clean and exact fashion without any appearance of thermal damage such as coagulation or vaporization. Instead, evidence is given that the tissue was very precisely etched, this kind of UV light induced ablation is called photoablation.

Typical threshold values of this type of interraction are $10^7-10^8 w/cm^2$ at laser pulse duration in the nanosecond range.

The main advantages: precision of the etching process, excellent predictability and the lack of thermal damage to adjacent tissue.

-----

@12.4

Photoablation can be summarized as a two-step process:

- Excitation: $AB+h\nu\rightarrow(AB)^*$
- Dissociation: $(AB)^*\rightarrow A+B+E_{kin}$

UV lasers, typically excimer lasers, provide an energy sufficient for dissociating such bonds.

The interaction mechanism of photoablation is limited to the application of uv light.

A certain threshold intensity must be applied to achieve photoablation. Above this intensity, a well-defined depth is ablated, depending on the absorption coefficient and the incident intensity. At the same time, an audible report is heard and visible fluoresconce is observed at the import site.

Principles of photoablation

- Absorption of high energy UV photos
- Promotion to repulsive excited states
- Dissociation 
- Ejection of fragments (no necrosis)
- Ablation

#### 3.3.1 model of photoablation

$$
I(z)=I_0\exp(-\alpha z)\\
z:\text{optical axis}\quad I_0:\text{incident laser intesity}\quad \alpha:\text{asorption coeffcient of tissue}\\
-\frac{\partial I}{\partial z}=\alpha I(z)\\
\alpha I(z)\ge \alpha I_{ph}\quad I_{ph}:\text{threshold intensity of photoablation}\\
I_0\exp(-\alpha z)\ge I_{ph}\\ d=\frac 1 \alpha\ln\frac{I_0}{I_{ph}}\approx\frac{2.3}{\alpha}\log_{10}\frac{I_0}{I_{ph}}
$$

Incident energy density $E_0 = I_0\tau$, $\tau$ is pulse duration

Plasma shielding: once a plasma is ignited at high power densities due to the generation of a high electric field, most of the succeeding laser radiation is absorbed by the plasma, thereby heating it up and leading to additional thermal effects.

In realitu, pure photoalbation is only observed for the 193nm wavelength of the ArF excimer-laser.

The significance of the thermal component increases with higher wavelengths - will be true in biological tissue.

#### 3.3.2 cytotoxicity of UV radiation

#### 3.3.3 summary of photoablation

Main idea: direct breaking of molecular bonds by high energy UV photons

Observations: very clean ablation, associated with audible report and visible fluorescence

Typical lasers: excimer laser, e.g. ArF, KrF, Xecl, XeF

Typical pulse durations: 10 — 100ns

Typical power densities: $10^7-10^{10}w/cm^2$

Special applications: refractive corneal surgery

### 3.4 plasma induced ablation

When obtaining power densities exceeding $10^{11}w/cm^2$ in solids and fluids or $10^{14}w/cm^2$ in air, a phenomenon called optical breakdown occurs.

By means of plasma induced ablation, very clean and well defined removal of tissue without evidence of thermal or mechanical damage can be achieved when choosing appropriate laser parameters.

Plasma induced ablation is also referred to as plasma mediated ablation.

-----

@12.11

The important feature of optical breakdown is that it renders possible an energy deposition not only in pigmented tissue but also in normally weakly absorbing media, this is due to the increased absorption coefficient of the induced plasma. In ophthalmology, transparent tissues-like cornea and lens-become potential targets of laser surgery.

#### 3.4.1 model of plasma induved ablation

Case I ($0\le t\le \tau$) :
$$
y\vec E_{th}=\frac s 2 +\sqrt{(\frac s 2)^2+\frac \tau {2\tau_c}}+\frac \tau {\tau_d}\\
y:\text{ionization probability}\quad \vec E_{th}: \text{threshold value of incident energy density}\\
y\vec I_{th}=\frac s {2\tau} +\sqrt{(\frac s {2\tau})^2+\frac 1 {2\tau\tau_c}}+\frac 1 {\tau_d}\\
\vec I_{th}:\text{threshold value of incident dencity}
$$
Case II ($t>\tau$) :
$$
\vec E_{th}\sim\tau^x\quad \vec I_{th}\sim\tau^{x-1}\\
x<0.1\quad \mathrm{for}\quad\tau<100fs\\
0.4<x<0.6\quad  \mathrm{for}\quad 4ps<\tau<8\mu s\\
x>0.8\quad  \mathrm{for}\quad \tau>300\mu s
$$
Free electron density:
$$
N(t)\approx N_{max}\exp(-\mathrm d t)=N_{max}\exp(-\frac t {\tau_d})
$$

#### 3.4.2 analysis of plasma parameters

#### 3.4.3 summary of plasma induced ablation

Main idea: ablation by ionizing plasma formation

Observation: very clean ablation associated with audible report and blueish plasma sparking

Typical lasers: Nd:YAG, Nd:YLF, TI:Sapphire

Typical pulse duration: 100fs—500ps

Typical power densities: $10^{11}-10^{13}w/cm^2$

Special applications: refractive corneal surgery, caries therapy

### 3.5 photodisruption

The physical effects associated with optical breakdown are plasma formation and shock wave generation. If breakdown occurs inside soft tissue or fluids, cavitation and jet formation may additionally take place.

When dicussing plasma induced ablation, we neglected any secondary effects of the plasma. At higher pulse energies - and thus higher plasma energies - shock waves and other mechanical side effects become more significant and might even determine the global effect upon the tissue.

Cavitation is an effect that occurs when focusing the laser beam not on the surface of a tissue but into the tissue.

In general, photodisruption may be regarded as a multi-cause mechanial effects starting with optical breakdown. The primary mechanisms are shock wave generation and cavitation, completed by jet formation if cavitations collapse in fluids and neal a solid boundary.

#### 3.5.1 plasma formation

The amount of energy absorbed during photodisruption is typical two or more orders of magnitude higher than during plasma induced ablation.

Plasma shielding -> Brillouin scattering -> multiple plasma generation

-----

@12.18

#### 3.5.2 shock wave generation

Cross section $A_0$      A shock front at a speed $U_s$
$$
u_s = \frac {\mathrm d x_s}{\mathrm d t}
$$
conservation of mass
$$
(\rho_1 -\rho_0)A_0\mathrm d x_s\\
u_p\rho_1A_0\mathrm d t=(\rho_1-\rho_0)A_0\mathrm d x_s\\
u_p=\frac{\rho_1-\rho_0}{\rho_1}u_s
$$
conservation of momentum
$$
A_0\rho_1u_p\mathrm d x_s
$$

- Mass $A_0\rho_1u_p\mathrm d t$ intruds at a speed up momentum $A_0\rho_1u_p^2\mathrm d t$
- $A_0(P_1-P_0)$ momentum $A_0(P_1-P_0)\mathrm d t$

$$
A_0\rho_1u_p\mathrm d x_s = A_0\rho_1u_p^2\mathrm d t+A_0(P_1-P_0)\mathrm d t\\
P_1-P_0=\rho_1u_su_p-\rho_1u_p^2
$$

$$
>20Kbar\quad u_s=1.483+25.306\log_{10}(1+\frac {u_p}{5.19})\\
<20Kbar\quad u_s=a+bu_p\\
a:\text{speed of sound}\quad b:\text{a diuensronless constant}\\
\text{water b=2.07}
$$

Assuming a spherical shock wave with radius $r$
$$
4\pi r^2\rho_1u_pu_s\Delta t=C_0\\
\Delta t:\text{risetime of shock front}\quad C_0:\text{constant}\\
u_s(u_s-a)=\frac{c_1}{r^2}\\
C_1=\frac b {4\pi\rho_1\Delta t}C_0\\
u_s(r)=\frac a 2 +\sqrt{\frac{a^2}{4}+\frac{C_1}{r^2}}\\
u_p(r)=-\frac a {2b}+ \frac 1 b\sqrt{\frac{a^2}{4}+\frac{C_1}{r^2}}\\
u_s=u_s(P_1)\quad u_p=u_p(P_1)\\
P_1(r)=P_0(r)+\frac{\rho_0C_1} b \frac 1 {r^2}
$$

$$
E_s\approx(P_1-P_0)A_s\Delta r\\
P_1:\text{shock wave pressure}\quad A_s:\text{shock wave surface}\\
\Delta r:\text{shock wave width}\\
A_s\approx 100\mu m^2 \text{for }30 ps,\quad E_s\approx0.5\mu J\\
A_s\approx 2500\mu m^2\text{for }6 ns,\quad E_s\approx50\mu J\\
$$

#### 3.5.3 cavitation

Laser induced cavitations occur if plasmas are generated inside soft tissues or fluids.

Rayleigh 1917:
$$
r_{\max}=\frac{t_c}{0.915\sqrt{\rho/(P_{stat}-P_{vap})}}\\
\begin{align}
&r_{\max}:\text{maximum radius of cavitation}\\
&\rho:\text{density of the fluid}\\
&P_{stat}:\text{static pressure}\\
&P_{vap}:\text{vapor pressure of the fluid}
\end{align}
$$

$$
E_b=\frac 4 3\pi(P_{stat}-P_{vap})r_{\max}^3
$$

It has been emphasized that damage of tissue due to shock waves is limited to a subcellular level due to their short displacement length of approximately $1-4\mu m$ since the diameter of cavitation bubbles may reach up to a few millimeters, microscopic photo disruptive effects inside tissue are believed to primarily originate from the combined action of cavitation and get formation.

#### 3.5.4 jet formation

When cavitation bubbles collapse in the vicinity of a solid boundary, a high speed liquid jet directed toward the wall is produced.

#### 3.5.5 summary of photodisruption

Main idea: fragmentation and cutting of tissue by mechanical forces

Observations: plasma sparking, generation of shock waves, cavitation, Jet formation

Typical lasers: solid, state lasers, e.g. Nd:YAG, Nd:YLF, Ti:Sapphire

Typical power densities: $10^{11}-10^{16}w/cm^2$

Typical pulse durations: $100fs-100ns$

Special applications: lens fragmentation, lithotripsy

-----

@12.25

# dental applications 

## 1. caries therapy

### 1.1 femtosecond laser based caries removal

1993 Niemz picosecond Nd:YLF

Lasers have NOT currently succeeded in replacing the dental drill in tooth hard tissue ablations due to slow material removal rates and unacceptable collateral damage.

Traditional drill is cheaper, more universal and faster than the laser, but it has an irritating sound, is unselective and not minimally invasive, transmits uncomfortable vibrations, creates heat and shock affecte zones despide cooling by air-water spray and thus pain, with need for local anesthesia.

#### 1.1.1 laser tissue interaction 

CPA Ti:Sapphire femtosecond laser

When comparing femtosecond laser dentistry with previous dental laser applications, the quality is primarily due to the single fact that femtosecond laser interaction with biological tissues is a direct multiphoton ionization of bound and free electrons, which leads to pure plasma induced ablation of the material.

This ultrafast and minimally invasive laser tissue interactions why the use of femtosecond laser pulses for tooth hard tissue ablation minimizes mechanical and thermal effects that precise sturcturing is possible without collateral injuries and most probably without activations of damage - sensing neurons, called no ciceptoss. 

#### 1.1.2 threefold caries selectivity

LIBS: laser induced breakdown spectroscopy

A first means of caries selectivity has been evaluated when comparing the ablation efficiencies of healthy and carious tooth substances.

A second means of caries selectivity is derived from the fact the pulse energy at the threshold of ablation is significantly lower when exposing carious surfaces.

A third means of caries selectivity becomes evident during optical spectroscopy of the laser induced plasma spark at the surface of the tooth.

### 1.2 retentive patterns at dentin surfaces facing filling meterials

Adhesion of restorative materials to the hard components of the tooth structure has been a goal pursued by numerous researchers ever since Buonocore establish the foundation for adhesive dentistry.

An improvement of retention can be achieved by creating patterns working as a micromechanical bond to the dental restoration. This kind of pattern is achieved by femtosecond laser application running under a defined scanning mode of beam.

### 1.3 intraoral application of a femtosecond laser beam

## 2. manufactoring of all ceramic restoration

If a large amount of tooth structure is lost or a whole tooth is lost, the first choise of therapy is to manufacture crowns and bridges fixed to the decayed teeth or to the adjacent teeth of the missing tooth.

Hot  isostatic-pressed(HIP) yttnia-tetragonal zirconia polgcrystal(Y-TZP) ceramic consists of fine particles of $ZrO_2$ and $Y_2O_3$, which when sintered, form a stable tetragonal structure at room temperature.

Processing $ZrO_2$ using a conventional laser cause microcracking. Using ultrafast laser pulses is an alternative possibility in processing HIP Y-TZP due to the nature of ultrashort laser pulses little or no collateral damage is expected.

