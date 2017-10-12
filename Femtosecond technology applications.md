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

Femtosecond  10^-15 s

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

