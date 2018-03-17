# Quantum Mechanic

## 1. 量子力学的诞生

### 1.1 无法用经典物理学解释的实验事实

#### 黑体辐射

**维恩（W. Wein）：**1896年，从热力学普适理论出发，结合试验数据，提出半经验公式
$$
E_\nu\mathrm d \nu=C_1\nu^3\exp(-C_2\nu/T)\mathrm d \nu
$$
其中$C_1C_2$是两个经验参数。获1911年诺贝尔奖。

**瑞利（J. W. Rayleigh）金斯（J. H. Jeans）：**1905年从波动理论和能量均分定理出发，推导出
$$
E_\nu\mathrm d \nu=KT\nu^2\mathrm d \nu
$$
Wein公式在短波部分与实验符合的很好，Rayleigh-Jeans公式在长波部分与试验符合的很好。

**普朗克（Planck）：**1900年10月19日发表拟合公式
$$
E_\nu\mathrm d \nu=\frac{C_1\nu^3}{\exp(C_2\nu/T)-1}\mathrm d \nu
$$
当$\nu\rightarrow\infty$时，
$$
\begin{align}
E_\nu\mathrm d \nu&=\frac{C_1\nu^3}{\exp(C_2\nu/T)-1}\mathrm d \nu\\
&\approx \frac{C_1\nu^3}{\exp(C_2\nu/T)}\mathrm d \nu\\
&=C_1\nu^3\exp(-C_2\nu/T)\mathrm d \nu
\end{align}
$$
得到Wein公式。当$\nu\rightarrow\infty$时，
$$
\begin{align}
E_\nu\mathrm d \nu&=\frac{C_1\nu^3}{\exp(C_2\nu/T)-1}\mathrm d \nu\\
&\approx \frac{C_1\nu^3}{1+(C_2\nu/T)-1}\mathrm d \nu\\
&=\frac{C_1}{C_2}T\nu^2\mathrm d \nu
\end{align}
$$
得到Rayleigh-Jeans公式。

![fig1.1 黑体辐射](https://i.loli.net/2018/01/17/5a5ebff6c781e.png)

#### 光电效应

**赫兹（Hertz）**：两个电荷间的相互作用，按照库仑力的解释是超距的，但按照麦克斯韦方程，电磁场的传播是需要时间的，Hertz为了验证麦克斯韦的说法，做了实验：

```sequence
participant 变压器\n(发射器)
participant 接收器
participant 金属板
变压器\n(发射器) -> 金属板: 行波
金属板 --> 变压器\n(发射器): 反射波
note over 接收器: 叠加形成驻波
```

移动接收器，测出波腹波节的位置，得到波长（6.6cm），说明麦克斯韦的电磁场理论正确。

> 有一天（1888年）Hertz做实验时，因为发射器的火花塞打火感到刺眼和烦躁，于是用木箱子罩住了发射器，但发现接收器在同一位置接收到的信号小了很多。Hertz没有放过这一现象，他换了几种不同的绝缘材料遮住发射器，均得到相同的结果，Hertz认为是光线中放出了某种东西，影响了接收器。他凭借着物理学家的直觉放下了手头重要的工作，专心研究这一现象。
>
> Hertz用一个三棱镜将发射器发出的光分成光谱，发现只有紫光和紫外光才会影响接收器。他断定是紫外光把接收器中某些带电的东西打了出来，使打火更容易了，并将这种现象命名为光电效应。

电子从金属中被打出来，一定是电磁波打到金属上，把能量传给电子，电子付出一部分脱出功，从金属中飞出。根据当时的理论，波的能量是跟振幅的平方有关的（光强），而与振幅无关。而实验现象表明只要光的频率在紫光以下，无论多大的光强都不能把电子打出来。

#### 原子的线状光谱

金属粉末在本生灯上燃烧，发出的光线经过光栅会被分成线状的、无规律（看似）的光谱。光谱作为一门经验科学发展的已经很好了，各种元素的谱线对应的波长都被精确的测定，人们可以通过观察材料的光谱确定其中含有的元素。

**巴尔末（Barlmer）**在1885年给出了氢原子一段光谱的公式：
$$
\frac 1 \lambda = R(\frac 1 {2^2}-\frac 1 {n^2})
$$

> Barlmer是一位瑞士的一位中学数学老师，瑞士冬天很冷，时间也很长，当地人在冬天出行困难于是经常在家做一些手工艺品（瑞士手表很出名可能与此有关），而Barlmer在家喜欢玩数学。比如给他一个数，他可以很快的告诉你这是哪两个素数之和，哪两个素数的平方之和，等等。
>
> 有一天他与化学家朋友Edward Hagenbach抱怨，已经穷尽了天下的数学，没有什么好玩的了，于是Edward就给了他一段氢原子光谱。Barlmer在两周之内就给出了巴尔末公式。

而物理学家对这个公式给不出任何解释，为什么谱线是分立的？为什么有的谱线亮，有的谱线暗？

#### 原子稳定性

>  1895年伦琴发现了x光，引起了很多学者对寻找射线的兴趣。巴黎自然博物馆职员Bequerrel作为一个研究地质的人，知道有些矿物质经过太阳暴晒之后会发荧光，于是就想到这些矿物会不会同时也在发出不可见光。他就把各种东西拿去暴晒，然后放在一个盒子里，在盒子上面放底片，看是否会曝光。
>
>  有一天他想把铀盐拿去暴晒，但正赶上天气不好，他就把铀盐先放在了箱子里，扔在柜子底部，而柜子上层刚好有一些胶片。经过二十几天，终于天气放晴，他把铀盐拿出去暴晒，并同时准备底片。严谨的Bequerrel想到底片在柜子里放了好久，可能会不小心曝光，于是决定冲洗一张看一下，结果令他大吃一惊，发现底片上有一个钥匙的图像。他去柜子里仔细一看，刚好在底层放铀盐的箱子和上层的底片中间有一个抽屉里装着一把钥匙。

Bequerrel发现了铀盐的天然放射性之后，1898年居里夫夫发现了放射性更强的镭，大家开始用镭做各种实验。

**卢瑟福（Rutherford）**让放射出的射线在电场中偏转，结果发现射线分成了三束，带正电的称为$\alpha$射线（其实是氦核），带负电的称为$\beta$射线（其实是高速电子），不偏转的称为$\gamma$射线（其实是电磁波）。这一工作很快便获得了诺贝尔奖。

Rutherford随后想到用分离出的$\alpha$粒子轰击铝箔、锡箔等，在硫化锌屏上观察$\alpha$粒子的偏转。

> Rutherford在曼彻斯特进行这一实验，在暗室中的荧光屏上看这些很暗的小亮点是十分痛苦的，身为老板的Rutherford便让他的研究生盖革来做这个实验。（痛苦的盖革下定决心发明计数器来代替自己，于是后来有了盖革计数器）盖革的工作是每天在实验室坐着，统计硫化锌屏上亮点的位置。有一天Rutherford突发奇想，让盖革把硫化锌屏换个位置观察，结果就发现了被铝箔反射回来的$\alpha$射线。

这对卢瑟福来说是不可理解的，因为当时对原子模型的理解是葡萄干面包模型，面包是正电荷，葡萄干是分布在其中的电子，而在这一模型下通过计算，脆弱的铝箔根本不可能把$\alpha$粒子弹回来。

于是Rutherford提出了新的原子模型：带正电的原子核十分小，在原子中间，周围是围绕着原子核转的电子。而根据这一模型计算的散射情况刚好可以符合轰击铝箔的实验现象。

但是，根据经典电动力学，围绕着原子核转动的电子是在做加速运动的，而做加速运动的电子会不断辐射出电磁波，不断损失能量，运动半径会越来越小，最终落到原子核上。

### 1.2 Planck-Einstein的光量子论

**普朗克（Planck）**四十二岁的时候，也就是1900年10月19日发表了公式：
$$
E_\nu\mathrm d \nu=\frac{C_1\nu^3}{\exp(C_2\nu/T)-1}\mathrm d \nu
$$
由于只提出了拟合公式，没有给出解释，所以没有在SCI索引刊物发表，只找了一篇核心刊物发表了：*M. Plank. Verh. D. Phys Ges 2, 202(1900)*。

于是Planck开始研究公式的推导，写出的论文与1900年12月4日寄出，1901年发表：*M. Plank, Ann der Physik 4, 553(1901)*。1900年12月4日也被认为是量子力学诞生的一天。
$$
\begin{align}
E_\nu\mathrm d \nu&=\frac{C_1\nu^3}{\exp(C_2\nu/T)-1}\mathrm d \nu\\
&=\frac{C_1\nu^3}{\exp(\frac{C_2k\nu}{kT})-1}\mathrm d \nu\\
&=\frac{kC_2\nu}{\exp(\frac{kC_2\nu}{kT})-1}\frac{C_1}{C_2k}\nu^2\mathrm d \nu\\
&=\bar\varepsilon_\nu\cdot N(\nu,\nu+\Delta\nu)
\end{align}
$$
即平均能量*允许的态的数量。
$$
\bar\varepsilon_\nu=\frac{kC_2\nu}{\exp(\frac{kC_2\nu}{kT})-1}=\frac{\mathrm d}{\mathrm d\beta}\ln[1-\exp(-\beta kC_2\nu)]\\
(\beta = \frac 1 {kT})
$$
这与统计力学中的平均能量
$$
\bar E = \frac{\sum_n \varepsilon_n e^{-\beta\varepsilon_n}}{\sum_ne^{-\beta\varepsilon_n}}= -\frac{\mathrm d }{\mathrm d \beta}\ln(\sum_ne^{-\beta\varepsilon_n})
$$
十分相似，假设二者是一样的则有
$$
\begin{align}
\sum_ne^{-\beta\varepsilon_n}=Z_\nu&=\frac 1 {1-e^{-\beta kC_2\nu}}\\
&=1+e^{-\beta kC_2\nu}+(e^{-\beta kC_2\nu})^2+...\\
&=1+e^{-\beta kC_2\nu}+e^{-2\beta kC_2\nu}+...\\
\end{align}
$$
对比两边，可以发现：
$$
\varepsilon_0 = 0,\quad\varepsilon_1 = kC_2\nu,\quad\varepsilon_2 = 2kC_2\nu,\quad...\quad\varepsilon_n = nkC_2\nu
$$
说明：驻波的能量不能是随意的，必须是$kC_2\nu$的整数倍。

令$kC_2=h$，则$\varepsilon_n=nh\nu$，$h$称为普朗克常数。

> 普朗克对这一结论并不相信，于是在论文中写的十分含糊，认为这只是一种说法，恰好能解释这个方程，而并不是真正正确的解释。
>
> Rayleigh-Jeans公式是在这之后五年才提出的，说明即使在五年后人们也没有相信普朗克是对的，仍然在试图用经典物理的方法进行解释。
>
> 当然也有人对普朗克的结论很认真，比如爱因斯坦。

1905年，爱因斯坦沿着普朗克的思路对光电效应做出了解释。

普朗克的假设是针对黑体辐射中的驻波的，Einstein将这一假设推广到了所有的电磁波，并引入了光量子（Light quanta）的概念，认为频率为$\nu$的电磁波辐射是由很多光量子组成的，每一光量子具有最小的能量
$$
E_\nu = h\nu=\frac h {2\pi}2\pi\nu = \hbar\omega
$$
根据狭义相对论，
$$
E^2=p^2c^2+m_0^2c^4
$$
对于电磁波，$m_0=0$，
$$
E^2 = P^2c^2\\
E=|\vec p|c\\
|\vec p|=\frac E c=\frac{h\nu} c=h\frac 1{cT}=\frac h \lambda=\frac h {2\pi} \frac{2\pi} \lambda =\hbar k\\
\vec p = \hbar\vec k
$$
光电效应可以这样理解：光量子的能量被电子吸收，电子付出一部分脱出功，从金属中逃逸以一定的动能逃逸
$$
\frac1 2 mv^2 = h\nu -A
$$
这就解释了当$\nu<\nu_0=A/h$时，不会发生光电效应的原因。

> 此后越来越多的人开始认真对待普朗克的量子假设。

### 1.3 Bohr的量子论

> 在量子力学史上，1911年发生了两件大事：第一件事是波尔（Niels Bohr）完成答辩，获得了博士学位；第二件事是Bohr紧接着订婚（与弟弟海拉德的同学的妹妹）了。
>
> Bohr是丹麦人，他的父亲是哥本哈根大学的一位生理学教授。据波尔回忆，他在两点上受父亲影响很深：一是小时候父亲经常带他出门玩，观察大自然；二是父亲与同事们每周末都会聚会，一群教授在某一个人家里一起吃饭闲聊，波尔与弟弟会在一边旁听，海阔天空的闲聊对Bohr有很大影响。
>
> > 波尔与弟弟小时候有些大智若愚的感觉，他们旁听教授们的聚会时一直是瞪着眼睛，有点呆呆的表情。据Bohr的母亲回忆，有一次带他们两个坐火车，母亲给他们读一本书，他们两个就傻傻的的聚精会神的听，到下车的时候旁边的一位老奶奶说：你抚养这么两个孩子真是太不容易了。
> >
> > （后来波尔的弟弟成为了著名的数学家，波尔就更不用说了）
> >
> > 两兄弟不但头脑厉害，四肢也发达，波尔的滑雪和足球都很厉害，是哥本哈根大学足球队的门将，弟弟是丹麦国家队的中锋。
>
> 1911年6月中旬，一个丹麦的啤酒商提供了一年的奖学金，订完婚的Bohr去了英国剑桥卡文迪许（Cavendish）实验室读博士后。因为波尔的博士论文就是研究电子的，而当时Cavendish实验室的领导人正是电子的发现者Thomson。
>
> 来到剑桥的Bohr想与Thomson聊聊，但Thomson当时忙于很多行政工作，与Bohr见面时桌上堆着两摞高高的文件，从文件中间的缝中，Thomson跟Bohr要了一份他的论文，然后堆在了文件顶上，很久都没有看。
>
> Bohr一个人待了半年，没有任何进展，情绪十分低落，一直到1912年2月，Rutherford来了。那时候Rutherford刚提出他的原子模型，在到处作报告，Bohr听完他的报告很感兴趣，去找卢瑟福说明了情况，说汤姆逊没什么时间管他，一年时间很快就结束了，希望能去跟卢瑟福做一段时间。
>
> 卢瑟福答应了他的请求，1912年4月波尔跟随卢瑟福来到曼彻斯特（Manchester），开始研究原子的稳定性问题。Bohr只用了两三个月的时间，就提出了一套理论，初步的解释了这个问题。

原子稳定性问题来源于电子围绕原子核的加速运动，于是Bohr提出了假设：

- 电子的状态不能连续的改变，只能处于某些分立的、确定的轨道上。改变轨道是以跳迁的方式，而不经历连续的过程。

- 在两个定态间跳迁是，原子吸收或发射的电磁波频率
  $$
  h\nu_{1,2}=E_1-E_2
  $$
























但很快他发现仅根据这两条假设不足以确定原子的分立能级，于是Bohr又引入了对应原理：即当量子数$n\rightarrow\infty$时，体系的行为应该是接近经典物理的。

基于以上三个假设，我们给出波尔的推导：

首先我们知道，氢原子是一个带正电的质子和一个电子组成的，电子处在库伦势
$$
V(r)=-\frac {e^2} r=-\frac \kappa r
$$
中的束缚态是一个椭圆轨道，其机械能$E<0$，长轴为$2a$，短轴为$2b$。由牛顿方程，容易得到：
$$
E = -\frac{\kappa}{2a},T^2 = \frac{4\pi^2ma^3}{\kappa}
$$

> 推导过程：考虑一个椭圆，近地点、远地点能量守恒和角动量守恒：
>
> ![fig1.2 椭圆](https://i.loli.net/2018/01/17/5a5f1e9949e7e.png)
> $$
> \begin{align}
> \frac12mv_1^2-\frac \kappa{r_1}=E=\frac 1 2 mv_2^2-\frac\kappa{r_2}\tag1\\
> mr_1v_1=L=mr_2v_2\tag2
> \end{align}
> $$
> 从（2）中解出$v_1v_2$代回（1）：
> $$
> \frac {L^2}{2mr_1^2}-\frac\kappa{r_1}=E=\frac {L^2}{2mr_2^2}-\frac\kappa{r_2}
> $$
> 左右两边分别乘$r_1^2$和$r_2^2$，得
> $$
> \begin{align}
> r_1^2E=\frac{L^2}{2m}-\kappa r_1\tag3\\
> r_2^2E=\frac{L^2}{2m}-\kappa r_2\tag4
> \end{align}
> $$
> （3）-（4），整理得
> $$
> E=-\frac\kappa{r_1+r_2}=-\frac\kappa{2a}
> $$
> （3）+（4），整理得
> $$
> \begin{align}
> (r_1^2+r_2^2)E&=\frac{L^2}{m}-2a\kappa\\
> L^2&=m[(r_1^2+r_2^2)E+2a\kappa]\\
> &= m[(r_1^2+r_2^2)E+2r_1r_2E-2r_1r_2E+2a\kappa]\\
> &=m[(r_1+r_2)^2E-2r_1r_2E+2a\kappa]\\
> &=m[4a^2E-2(a-c)(a+c)E+2a\kappa]\\
> &=m[4a^2E-2(a^2-c^2)E+2a\kappa]\\
> &=m[4a^2E-2b^2E+2a\kappa]\\
> \end{align}
> $$
> 又因为$E=-\kappa/2a$，则其中两项消掉，
> $$
> \begin{align}
> L^2&=-2mb^2E\\
> &=\frac{\kappa b^2} a m
> \end{align}
> $$
> 为了将角动量与时间联系起来，我们分析椭圆上某点的运动状态：
>
> ![fig1.3 椭圆](https://i.loli.net/2018/01/17/5a5f22dba3903.png)
> $$
> \begin{align}
> L& = |\vec r \times \vec p|=rmv\sin\theta\\
> &=\lim_{\Delta t\rightarrow 0}rm\frac{\Delta s}{\Delta t}\sin(\pi-\alpha)\\
> &=\lim_{\Delta t\rightarrow 0}m\frac{\Delta s}{\Delta t}r\sin\alpha\\
> &=\lim_{\Delta t\rightarrow 0}2m\frac{\Delta S}{\Delta t}\\
> &=2m\frac{\mathrm d S}{\mathrm d t}
> \end{align}
> $$
> 这样就得到了角动量与时间的关系：角动量等于单位时间内矢径扫过的面积乘以2m。对该式两边积分，就得到开普勒第二定律：
> $$
> \begin{align}
> \int_0^TL\mathrm d t&=\int_0^T2m\frac{\mathrm d S}{\mathrm d t}\cdot\mathrm d t\\
> LT&=2m\int_{椭圆}\mathrm d S=2m\pi a b\\
> \end{align}
> $$
> 则得到周期与角动量的关系：$ T = 2m\pi ab/L$，与上面的式子联立，即得出最终结果：
> $$
> T^2=\frac{4m^2\pi^2a^2b^2}{\frac{\kappa b^2}{a}m}=\frac{4\pi^2ma^3}{\kappa}
> $$
>

有了这两个式子之后，我们消去其中的a：
$$
T^2=\frac{4\pi^2m}\kappa(-\frac\kappa{2E})^3=\frac{\pi m\kappa^2}{2|E|^3}
$$
注意到能量是负数，所以加个负号即为绝对值。得到了周期之后，其倒数就是轨道频率
$$
\nu=\frac 1 T=\frac 1{\pi\kappa}\sqrt{\frac 2m}(-E)^{2/3}
$$
对一个特定轨道来说，可以表示为
$$
\nu(n)=\frac 1 T=\frac 1{\pi\kappa}\sqrt{\frac 2m}(-E(n))^{3/2}
$$
根据Bohr的第二条假设，当一个电子从第n条轨道跳迁至第n-1条轨道时，放出的电磁波由如下关系决定：
$$
h\nu_{n,n-1}=E(n)-E(n-1)\approx E^\prime(n)\Delta n=E^\prime(n)
$$
为了求解这个倒数，令$E(n)=h\nu(n)f(n)$，注意普朗克常数乘频率是具有能量量纲的，所以$f(n)$是一个无量纲的数
$$
\begin{align}
f(n)&=\frac{E(n)}{h\nu(n)}\\
f^\prime(n)&=\frac{E^\prime(n)}{h\nu(n)}+\frac{E(n)}{h}\frac{\mathrm d}{\mathrm d n}(\frac 1 {\nu(n)})\\
&=\frac{E^\prime(n)}{h\nu(n)}+\frac{E(n)}{h}\frac{\mathrm d}{\mathrm d E}(\frac 1 {\nu(n)})\frac{\mathrm d E}{\mathrm dn}\\
&=\frac{E^\prime(n)}{h\nu(n)}+\frac{E(n)}{h}\frac{\mathrm d}{\mathrm d E}(\frac 1 {\nu(n)})E^\prime(n)\\
&=\frac{E^\prime(n)}{h\nu(n)}+\frac{E(n)}{h}(-\frac 1 {\nu^2(n)})\frac{\mathrm d \nu(n)}{\mathrm d E}E^\prime(n)\\
&=\frac{E^\prime(n)}{h\nu(n)}[1-E(n)\frac 1{\nu(n)}\frac{\mathrm d\nu(n)}{\mathrm d E}]\\
&=\frac{E^\prime(n)}{h\nu(n)}[1-E(n)\frac{\mathrm d\ln\nu(n)}{\mathrm d E}]\\
\end{align}
$$
考虑对应原理，当量子数n足够大的时候，得出的结论应该是趋于经典的，而根据电动力学给出的结论，这时辐射出电磁波的频率高好就等于绕核运动的轨道频率
$$
E^\prime(n)=h\nu_{n,n-1}\approx h\nu(n)\\
\frac{f^\prime(n)h\nu(n)}{1-E(n)\frac{\mathrm d\ln\nu(n)}{\mathrm d E}}=h\nu(n)\\
f^\prime(n)=1-E(n)\frac{\mathrm d\ln\nu(n)}{\mathrm d E}
$$
式中$\ln\nu(n)$与$E$的关系之前已经给出，只需两边取对数并求导：
$$
\nu(n)=\frac 1{\pi\kappa}\sqrt{\frac 2m}(-E(n))^{3/2}\\
\ln\nu(n)=\ln(\frac 1{\pi\kappa}\sqrt{\frac 2m})+\frac32\ln(-E(n))\\
\frac{\mathrm d \ln\nu(n)}{\mathrm d E}=0+\frac32\frac1 {-E(n)}(-1)\\
\frac{\mathrm d \ln\nu(n)}{\mathrm d E}=\frac 3{2E(n)}
$$
带入上式，得
$$
f^\prime(n)=1-E(n)\frac32\frac 1 {E(n)}=-\frac 12
$$
积分：
$$
f(n)=-\frac 12n+D
$$
则回到最开始的时候，
$$
E(n)=h\nu(n)f(n)=h[\frac 1{\pi\kappa}\sqrt{\frac 2m}(-E(n))^{3/2}][-\frac12n+D],\kappa=e^2\\
E(n)=-\frac{\pi^2e^4m}{2h^2(-\frac12n+D)^2}
$$

>  注意推导中的条件说明这个式子在n很大的时候是成立的，而当n很小的时候Bohr就没有办法了，所以他就做出了一个大胆的假设：当n很小时也成立。

这样波尔的计算就很好的解决了原子稳定性问题：只有满足上述公式的能量才是可以稳定存在的允许态，而这个能量有一个最小值，当电子跳迁至这一能量最小轨道时将不能继续辐射电磁波。

> Bohr很高兴的拿着这一成果去找Rutherford，而卢瑟福对波尔得假设感到很不满，他认为波尔的几条假设暗含了原子稳定，形成了逻辑循环，他就跟Bohr说，你看你，四月份来的，这才七月份，就做出了这么重要的成果……要不你再回去考虑考虑？Bohr则以一年的奖学金即将到期为由想要拒绝，卢瑟福表示钱不是问题，他可以去英国皇家学会给Bohr再申请一年的奖学金，让Bohr再留下了做一年，看看能不能把他的假设去掉一些，用更自然的方式推导出结果。
>
> 此时的Bohr面临着两难的境地：一方面教授不让他发表文章，一方面不知道继续做下去该做什么。于是一年前订了婚的Bohr选择了回家结婚。
>
> 现在我们知道，原子的稳定性问题背后是有很深刻的物理原理的（测不准原理），即使波尔留下来在做一年也基本上是不可能解决的。而恰恰是他选择了回家结婚，遇到了一位友人，使Bohr漂亮的完成了他的工作。
>
> 大概1912年的8月，波尔回家结婚，然后去度蜜月，10月度完蜜月回来，准备重新考虑氢原子的稳定性问题，这时遇到了Hanssen，一位研究光谱的人，Hanssen给了他巴尔末公式，让他考虑一下氢原子光谱问题。后据Bohr所说，他一看到巴尔末公式里的$n^2$，他就全明白了。

令常数$D=0$，
$$
E(n)=-\frac{2\pi^2e^4m}{n^2h^2}
$$
考虑电子从高层轨道向$n=2$的轨道跳迁的情况：
$$
E(n)-E(2)=\frac {2\pi^2e^4m}{h^2}(\frac 1 4-\frac 1{n^2})=h\nu_{n,2}=h\frac 1 {T_{n,2}}=\frac{hc}{cT_{n,2}}=\frac{hc}{\lambda_{n,2}}\\
\frac 1 {\lambda_{n,2}}=\frac{2\pi^2e^4m}{h^3c}(\frac14-\frac1{n^2})
$$
与巴尔末公式相比：
$$
\frac 1\lambda=R(\frac14-\frac1{n^2})
$$
实验测得的常数值与推导出的结果符合的相当好
$$
\frac{2\pi^2e^4m}{h^3c}=R
$$

>  这是自1885年巴尔末猜出这一段光谱公式之后首次给出推导，Bohr赶紧把这一结果写信告诉了卢瑟福，卢瑟福也马上意识到Bohr的工作的重要意义，很快就同意了Bohr论文的发表：N. Bohr, On the Constitution of atoms and molecules. Phil Meg 26,1025 (1913)。
>
>  今天有很多物理学家认为Bohr的这一成果是20世纪最伟大的物理成果，甚至比爱因斯坦的相对论还要伟大。当时人们高兴的认为，Bohr已经把大门打开了，接下来将会一路畅通，但很快大家就发现并不是这么回事。只有氢原子可以用Bohr的方法求解，从氦开始就行不通了。
>
>  1913年到1925年，量子力学一直在这一困境中没有什么进展。

### 1.4 Heisenberg和Dirac的矩阵力学

> 海森堡的父亲对拜占庭的文化非常感兴趣，创办了一份杂志，叫做拜占庭文化研究，自任主编。海森堡的父亲交友广泛，1919年海森堡高中毕业，对数学很感兴趣，甚至看过H. Weyl的Space, Time and Matter，于是父亲就找到了一位数学系主任Lindemann（第一个证明了圆周率是超越数）。海森堡与Lindemann的会面并不愉快，因为老教授的听力不太好，海森堡也比较紧张，甚至连教授听没听懂他的话都不清楚。但Lindemann至少问了他一个问题：你说喜欢学数学，那你看过哪些数学的书呢？海森堡回答，看过Space, Time and Matter。Lindemann当即表示，完了完了，你绝对不要再学数学了，你已经被Weyl彻底毁掉了。海森堡很丧气的回家了，但朋友很多的父亲又给他找了另一个朋友：理论物理研究所的索末菲尔德（Sommerfeld）。索末菲尔德是一个很热情的人，也问了海森堡同样的问题，海森堡也说了同样的答案，而索末菲尔德的答案完全不同，他很惊讶的表示你竟然读这么深奥的东西，我都没有读过。索末菲尔德也劝告海森堡，不要太性急，急着讨论物理背后的哲学是没有意义的，应该从简单的计算入手，来慢慢得到一个图像。
>
> 当然索末菲尔德录取了海森堡。Sommerfeld是一位非常好的老师，他给他的学生亲自授课，在课堂上海森堡结识了泡利，二人都对量子力学的发展做出了重要的贡献。
>
> 海森堡与泡利讨论过有什么值得做的课题，泡利说相对论已经差不多到头了，你可以研究一下原子物理。Sommerfeld也给出了同样的建议，但是当时他说原子物理太难了，先给了海森堡一个湍流的课题。海森堡后来回忆，幸好没有在湍流里陷得太深，否则这东西就做不完了。
>
> 1922年格丁根大学的波恩和希尔伯特联合发出邀请，请波尔从丹麦过来做一周的演讲，详细的讲解了原子光谱、量子论等问题。演讲过程中海森堡提了一个问题，令Bohr印象深刻，于是在演讲结束后Bohr邀请他一起出去散步。两人沿着格丁根旁边的一个小山一直走到山顶，Bohr还邀请他到自己那里做半年的交换学生。
>
> > 1942年10月，两人最后一次散步成为了重要的历史事件。当时丹麦已经被希特勒占领，算不准先生海森堡算错了铀原子弹的临界质量，他跟波尔说，原子弹这个东西，弄不了的。而波尔听到这句话，脸色大变，马上表示不要再散步了，就回去了。据波尔回忆，他听到的是海森堡在暗示德国马上就要造出原子弹了，海森堡好像是来劝降的。当时德国虽然占领了丹麦，但是对这些科学家并没有什么动作，而这个时候波尔觉得他必须逃跑了，Bohr乘着小船和全家跑到了瑞典，瑞典当时是一个中立国，并不足够安全，他把夫人和孩子留在瑞典，本人继续逃亡。英国方面派了一个轻型轰炸机，把他装在弹舱里运走。飞行员给了Bohr一副耳机让他带上，因为刚开始飞行的时候为了躲避雷达是低空飞行的，而飞一段时间之后为了省油要高空飞行，这时候会用耳机通知他带上氧气面罩。Bohr由于脑袋比较大，耳机没有带好，错过了带氧气面罩的通知，于是就昏迷了，经历了二十几分钟的高空飞行，飞机在苏格兰下降，Bohr又苏醒了过来。
>
> 1923年毕业（四年，本科+研究生）的海森堡在答辩会上差点没有通过，因为答辩老师Wein问了他几个实验上的问题他都没有答上来，Wein很生气的要给他一个D，后来索末菲尔德去求情，才给了C。
>
> 泡利毕业之后Sommerfeld就把他派去了波恩那里做助手，泡利呆了不到一年就被Bohr弄走了，波恩给索末菲尔德写信说，大概再也遇不到这么好的学生了，Sommerfeld就把海森堡派了过去。
>
> 海森堡回忆说，他从索末菲尔德那里学到了物理，从波尔那里学到了思想，从波恩那里学到了数学。
>
> 1925年6月7日，他由于枯草热不得不停下手头的工作前往北海的一个小岛，Helgoland。这使得他有时间重新考虑Bohr量子论的基础。有一天早上他在海边看太阳，随着太阳的冉冉升起，他脑海中突然产生了一些想法：
>
> 所有可观测的物理量都是与两条Bohr轨道有关的。如此一来每个动力学变量都应由一个矩阵（当时海森堡并不知道那是矩阵）表示，每个矩阵元都与两个态有关。
>
> 海森堡试图用它新发明的这种方法计算一维谐振子问题，他很快发现了不可对易的问题，但他用数学方法绕了过去，写出了一篇十分难懂的文章，很快在7月份就发表了，史称一人文章。而后他的老师波恩很快认识到海森堡说的其实就是矩阵，于是他让他的博士后P. Jordan去计算$\hat x\hat{P_x}-\hat{P_x}\hat x$，约旦在两星期内就给出了答案，并发表了文章，称为二人文章。波恩把这一进展写信告诉了海森堡，海森堡赶回学校他们一起写了一篇综述，称为三人文章。
>
> 但是Jordan的推导十分依赖于一维谐振子的性质，对于氢原子就无计可施了，真正给出普遍推导的是狄拉克（Dirac）。
>
> Dirac的父亲脾气十分暴躁，在家吃饭的时候是母亲带着哥哥和妹妹在厨房吃饭，Dirac和父亲单独吃，父亲要求他在家要讲法语，而只要Dirac说话犯了一个语法错误，父亲上去就会给他一耳光。他们父子关系闹得很僵，以至于后来Dirac得诺贝尔奖的时候只让母亲去了，都没有让父亲参加。
>
> 这让Dirac从小养成了一个习惯：说每句话之前都要仔细想好了再说。Dirac的一生也是沉默寡言的，以至于有人怀疑他是自闭症。1919年16岁的Dirac进了Bristol本地的一个大学念电机工程，因为Dirac虽然对数学很感兴趣，但他认为念纯数学可能会找不着工作。念了三年之后Dirac因为没找到工作，只好拿着数学系的奖学金又去念了两年数学。1923念毕业之后剑桥给了一份奖学金，Dirac才开始跟着导师Fowler从事物理工作。
>
> Fowler也是一位很著名的物理学家，是卢瑟福的女婿，擅长各种球类运动，尤其是高尔夫。Fowler给Dirac的第一个题目是：溶解速度是否会受温度梯度的影响。学了一年之后，Fowler开始给他一些重要的工作，时值1925年，海森堡的文章已经出来了。剑桥大学卡文迪许实验室有一个卡皮猹俱乐部，海森堡去做了一个报告，并留下了几个文章的印本。Fowler拿到了一本，他很感兴趣，于是就让Dirac读一读，自己去打高尔夫。Dirac读了两星期都没有读懂，直到Fowler问他这篇文章都说了什么的时候，Dirac告诉他这篇文章都是垃圾（Rubbish）。
>
> 于是Dirac抱着要推翻海森堡的理论体系的目的试图自己计算$\hat x\hat{P_x}-\hat{P_x}\hat x$

首先Dirac引入了一个记号：
$$
\hat A\hat B -\hat B \hat A =[\hat A,\hat B]
$$
称为对易子（commutator）。Dirac发现了对易子满足的一些关系：
$$
\begin{align}
[\hat u,\hat v]=-[\hat v, \hat u]\tag i\\
[\hat u, C\hat I]=0\tag {ii}\\
[\hat u_1+\hat u_2,\hat v]=[\hat u_1, \hat v]+[\hat u_2,\hat v]\tag{iii}\\
[\hat u,\hat v_1+\hat v_2]=[\hat u,\hat v_1]+[\hat u,\hat v_2]\tag{iv}\\
[\hat u_1\hat u_2,v]=[\hat u_1,\hat v]\hat u_2+\hat u_1[\hat u_2,\hat v]\tag{v}\\
[\hat u,\hat v_1\hat v_2]=[\hat u,\hat v_1]\hat v_2+\hat v_1[\hat u,\hat v_2]\tag{vi}\\
[\hat u,[\hat v,\hat w]]+[\hat v,[\hat w,\hat u]]+[\hat w,[\hat u,\hat v]]=0\tag{vii}
\end{align}
$$

> Dirac在这些代数中挣扎了很久，没有取得更多的进展，他习惯周一到周六工作，周日郊外远足，突破就出现在他的一次远足中：他突然想到这些东西他好像在哪里见过。他用排除法推测应该是在自学分析力学的时候见过，于是Dirac回到家急急忙忙的找分析力学的书，结果一本也没有找到，那天晚上是他一生中最漫长的一个晚上，第二天图书馆的门一开，他就匆匆忙忙的冲到图书馆找到一本分析力学的书，发现了泊松(Poisson)括号。
$$
{u,v}=\sum_i(\frac{\partial u}{\partial q_i}\frac{\partial v}{\partial p_i}-\frac{\partial u}{\partial p_i}\frac{\partial v}{\partial q_i})
$$
这里，u和v是任意两个广义坐标与广义动量（$q_1,q_2,\dots,q_N,p_1,p_2,\dots,p_N$）的函数。

Poisson括号也满足上面的七个关系。Dirac下一步就想到了Bohr的对应原理，泊松括号里的是经典力学量，对易子里的是量子力学的矩阵表示，他们之间一定是有联系的。Dirac认为他们应该是成正比的：
$$
[\hat u,\hat v]=D{u,v}\hat I
$$
而这个D应该是与量子力学特征值$\hbar$有关的一个常数。从量纲的角度说，$[\hbar]=[E][T]$，当体系足够宏观的时候，可以认为$\hbar\rightarrow 0$，则等式右边就变成了0，对易子等于0则表示两个物理量可以对换，就变成了经典物理结果。

> Bohr的量子论中唯一可靠的就是氢原子能级公式，因为有光谱实验可以证明，所以Dirac的问题就变成了用泊松括号的表示形式推出氢原子能及公式，与光谱实验比较就可以定出常数D，这一推导十分困难，最终是由泡利完成的。
>
> Pauli的父亲是维也纳大学的一位化学教授，有很多的好朋友，其中一位就是哲学系教授、物理系教授马赫，马赫也是Pauli的教父。Pauli是一位神童，从小就看了很多书，尤其对相对论很感兴趣，以至于当他18岁去索末菲尔德那里读大学的时候已经是公认的广义相对论专家了。索末菲尔德当时承担了一个任务，要给德国物理学会编一套百科全书，其中广义相对论的那一卷就请了当时19岁的Pauli来写，写了三百多页。也是在这个东西做完之后他跟海森堡说广义相对论没什么好搞的了，他本人之后也很少去碰广义相对论。

Pauli经过复杂的计算定出了常数D的值$D=i\hbar$，即
$$
[\hat x,\hat p_x]=i\hbar\hat I
$$
称为量子力学基本方程式。

> 直接利用矩阵进行计算是一件很复杂的事情，而且当时的物理学家大都是不懂矩阵的，所以矩阵力学发展十分缓慢，幸运的是几乎在同时，德布罗意（De Broglie）和薛定谔（Schrodinger）发展了一套等价的波动力学。波动力学体系最大的好处是以微分方程的形式出现的，而微分方程是所有物理学家都会的。

### 1.5 Wave Machanics

> 德布罗意是法国人，名字里的De表示是贵族，意思是从什么家族来的，类似的在德国是Von，在荷兰是Van，但也有可能表示是从某个村子里来的村民。自从法国大革命之后，大部分贵族都被干掉了，也有很多家道败落，但德布罗意家还好得很，他的父亲是当时法国的一个国务部长，富有的家境使De Broglie有大把的空闲时间，但他并不是游手好闲无所事事的人，他对“谜一般的东西”十分感兴趣，比如中世纪史，Broglie花了很多时间研究中世纪史，但有一天他突然觉得这个东西没劲了，他读到了一些普朗克、爱因斯坦的文章，觉得物理很有意思，决定转学物理，于是就找到了一位老师：朗之万（Langevin）。朗之万是居里夫人的学生，当时已经是很有名的物理学家，而且不像大部分不通人情世故的物理学家，朗之万听说Broglie是国务部长的儿子，马上就答应了他来学习。
>
> 德布罗意看了爱因斯坦的光电效应解释之后，提出了一个异想天开的想法：电磁场可以写成波函数，为什么电子不可以也看作是波呢？

电磁场的波函数我们都很熟悉：
$$
E = \vec E_0 \exp [i\vec k_0\cdot\vec r-i\omega t]
$$
这是一个矢量波，德布罗意就假设电子可以写成一个标量波的形式：
$$
\psi(\vec r,t)=\psi_0\exp[i\vec k\cdot\vec r-i\omega t]
$$
其能量和动量也由普朗克爱因斯坦关系与频率和波矢建立联系：
$$
E=\hbar\omega\\
\vec p=\hbar\vec k
$$

这一奇怪的想法似乎又是很有道理的，德布罗意考虑了这样一个特例：

一个绕着氢原子核运动的电子（时值1924年，海森堡的理论还没有提出，人们仍按Bohr的老量子论认为电子是以一定轨道运行的），电子的角动量是守恒的，其大小、方向都不变，那么电子一定是在与角动量垂直的平面内运动，将椭圆轨道简化为圆轨道，那么假如电子也是一种波的话，它会在轨道上形成一个驻波，如图所示。

![fig 1.4 电子波](https://i.loli.net/2018/01/24/5a68438c0daea.png)

显而易见，要想形成驻波，圆轨道的周长必须是波长的整数倍：
$$
2\pi R=n\lambda,\quad n=1,2,3,\dots
$$
考虑其动量：
$$
L=Rp=R\hbar k=R\hbar\frac{2\pi}{\lambda}=R\hbar\frac{2\pi}{\frac{2\pi R}{n}}=n\hbar
$$
这就是Bohr的角动量量子化条件。

> 这一发现让Broglie很兴奋，索性就把它写成了论文送给了朗之万。朗之万看到了论文就开始头痛了，因为德布罗意要毕业，论文也写出来了，就这么多：波就是粒子，粒子就是波。朗之万很难受，他要是不让德布罗意毕业，那等于是搬起石头砸自己的脚，因为当初收他进来就是要做个人情。要是让德布罗意毕业，也很麻烦，因为答辩委员会有五个人，其中有两个是做实验的。答辩时这两个做实验的老师也确实当场提出了反对，因为这个东西没法用实验验证。
>
> 朗之万毕竟是非常聪明的人，他为了让德布罗意顺利毕业，给爱因斯坦打了个电话，说我这里有一个学生，他把您的关于电磁波的理论给推广了，推广到了一般的物质波，请您好好的阅读一下，给一个中肯的意见，顺便说一声，这个学生的父亲是我国很重要的一位国务部长，以后您到敝国来的时候，一定会收到敝国政府热情的欢迎。
>
> 爱因斯坦显然也是非常聪明的人，在他给朗之万的回信中表扬了De Broglie，也给答辩委员会写了评语，类似“德布罗意天才的、创造性地发挥了我的思想，将这些关系式从电磁波推广到了物质波，使得我过去提出的理论大大的向前迈进了一步，我认为这篇文章应该被评为贵国的优秀博士论文”。
>
> 朗之万拿到爱因斯坦的回信赶紧把信给委员会其他四个人看了，那两位持坚决反对意见的老师马上态度就变了，因为就连爱因斯坦都给出了如此表扬，他们反对显然是没能很好的读懂这篇文章的真实含义。于是德布罗意于1924年顺利毕业，拿到了巴黎大学的博士学位。
>
> 德布罗意在此之后也没怎么从事物理方面的工作，转而研究生物。然而幸运的是事情并没有到此结束，按照当时的习惯，接下来巴黎大学要把这篇博士论文送到各大大学去，其中有一份就送到了瑞士苏黎世高工（ETH）。当时ETH有一位物理学教授，德拜（Debye），他是索末菲尔德的学生，索末菲尔德有四位获得了诺贝尔奖的学生，他就是其中一位。Debye当时在组织一个报告会，有很多周围学校的老师学生也会来听，在苏黎世大学的38岁的高级讲师薛定谔也来听了这个报告。会后Debye把德布罗意的论文给了薛定谔，让他回去看一看，两个星期之后来交流一下。两个周之后薛定谔给出了一个报告，报告的主要内容就是粒子就是波，波就是粒子。所有人都听的一头雾水，当时Debye就给了一个建议，他说他的老师索末菲尔德曾经说过，你想要深刻的了解一种波，你就要把它的波动方程写出来。
>
> 薛定谔深以为然，回去研究了一下这个波动方程，给出了薛定谔方程。

薛定谔从一个自由粒子的角度出发，大家都知道
$$
E=\frac{p^2}{2m}
$$
在这个方程的两边乘上波函数
$$
\begin{align}
E\psi(\vec r,t)&=\frac{p^2}{2m}\psi(\vec r,t)\\
E\psi_0\exp(i\vec k\cdot \vec r-i\omega t)&=\frac{p^2}{2m}\psi_0\exp(i\vec k\cdot \vec r-i\omega t)\\
\hbar\omega\psi_0\exp(i\vec k\cdot \vec r-i\omega t)&=\frac{(\hbar\vec k)^2}{2m}\psi_0\exp(i\vec k\cdot \vec r-i\omega t)\\
\frac\hbar{-i}\frac{\partial}{\partial t}\psi_0\exp(i\vec k\cdot \vec r-i\omega t)&=-\frac{\hbar^2}{2m}\nabla^2\psi_0\exp(i\vec k\cdot \vec r-i\omega t)\\
i\hbar\frac\partial{\partial t}\psi(\vec r,t)&=-\frac{\hbar^2}{2m}\nabla^2\psi(\vec r,t)
\end{align}
$$

> 写出了波动方程的薛定谔很高兴的找到了Debye，Debye又让他做了一个报告，但人们仍不知道这有什么意义。薛定谔想到，要证明这个东西是正确的，他必须由此推出氢原子能级公式。

他首先改写了这个方程，因为上面的方程是基于自由电子的，而氢原子中的电子显然是束缚的，那么从一开始就应该把势能考虑进去：
$$
E=\frac{p^2}{2m}+v(r)
$$
由此得到的波函数是
$$
i\hbar\frac\partial{\partial t}\psi(\vec r,t)=-\frac{\hbar^2}{2m}\nabla^2\psi(\vec r,t)+v(r)\psi(\vec r,t)
$$
氢原子中的$v(r)$应该是$-e^2/r$，即
$$
i\hbar\frac\partial{\partial t}\psi(\vec r,t)=-\frac{\hbar^2}{2m}\nabla^2\psi(\vec r,t)-\frac{e^2}{r}\psi(\vec r,t)
$$
用分离变量法求解，首先令
$$
\psi(\vec r,t)=\Phi(\vec r)f(t)=\Phi(\vec r)e^{-i\omega t}
$$
其中$\omega$是待定常数。代入方程，得到
$$
\begin{align}
i\hbar\frac\partial{\partial t}\Phi(\vec r)e^{-i\omega t}&=-\frac{\hbar^2}{2m}\nabla^2\Phi(\vec r)e^{-i\omega t}-\frac{e^2}{r}\Phi(\vec r)e^{-i\omega t}\\
i\hbar\Phi(\vec r)\frac\partial{\partial t}e^{-i\omega t}&=[-\frac{\hbar^2}{2m}\nabla^2\Phi(\vec r)-\frac{e^2}{r}\Phi(\vec r)]e^{-i\omega t}\\
i\hbar(-i\omega)\Phi(\vec r)e^{-i\omega t}&=[-\frac{\hbar^2}{2m}\nabla^2\Phi(\vec r)-\frac{e^2}{r}\Phi(\vec r)]e^{-i\omega t}\\
\hbar\omega\Phi(\vec r)&=-\frac{\hbar^2}{2m}\nabla^2\Phi(\vec r)-\frac{e^2}{r}\Phi(\vec r)
\frac{e^2}{r}\Phi(\vec r)]e^{-i\omega t}\\
E\Phi(\vec r)&=-\frac{\hbar^2}{2m}\nabla^2\Phi(\vec r)-\frac{e^2}{r}\Phi(\vec r)
\end{align}
$$
这样就得到一个不含时间的方程，称为定态方程。这个方程一般是没有解的，除非E取某些特定的值，这类问题称为本征值（Eigenvalue）问题。由于这是一个向心力场下的问题，所以我们用球坐标，在球坐标下，拉普拉斯算符可以写作
$$
\nabla^2=\frac 1 {r^2}\frac\partial{\partial r}r^2\frac\partial{\partial r}+\frac1{r^2}[\frac{1}{\sin\theta}\frac\partial{\partial\theta}(\sin\theta\frac\partial{\partial\theta})+\frac 1 {\sin^2\theta}\frac{\partial^2}{\partial\varphi^2}]
$$
则薛定谔方程可以写为
$$
E\Phi(\vec r)=E\Phi(r,\theta,\varphi)
\\=-\frac{h^2}{2m}\frac 1 {r^2}\frac\partial{\partial r}r^2\frac\partial{\partial r}\Phi(\vec r)-\frac{h^2}{2mr^2}[\frac{1}{\sin\theta}\frac\partial{\partial\theta}\sin\theta\frac\partial{\partial\theta}+\frac 1 {\sin^2\theta}\frac{\partial^2}{\partial\varphi^2}]\Phi(r,\theta,\varphi)-\frac{e^2}r\Phi(r,\theta,\varphi)
$$
我们使用球谐函数继续分离变量。

> 球谐函数的定义
> $$
> Y_{LM}(\theta,\varphi)=(-1)^M\sqrt{\frac{(2L+1)(L-M)!}{4\pi(L+M)!}}P_L^M(\cos\theta)e^{iM\varphi}
> $$
> 其中$L=0,1,2,\dots$，$-L\le M\le L$，$P_L^M$称为连带雷让德（Legendre）函数。
>
> 首先定义雷让德函数
> $$
> P_L(x)=\frac1{2^LL!}\frac{\mathrm d^L}{\mathrm d x^L}(x^2-1)^L
> $$
> 连带雷让德函数
> $$
> P_L^M(x)=\frac1 {2^LL!}(L-x^2)^{M/2}\frac{\mathrm d^{L+M}}{\mathrm d x^{L+M}}(x^2-1)^L\\
> =(1-x^2)^{M/2}\frac{\mathrm d^M}{\mathrm d x^M}P_L^M(x),\quad M\ge0\\
> P_L^{-M}(x)=(-1)^M\frac{(L-M)!}{(L+M)!}P_L^M(x)
> $$
> 引入这些因子之后，我们可以得到一个简单的积分形式：
> $$
> \int_{-1}^1P_{L1}(x)P_{L2}(x)\mathrm d x=\frac2{2L+1}\delta_{L1L2}\\
> \int_)^\infty\int_0^\pi\int_0^{2\pi} Y^*_{L'M'}(\theta,\varphi)Y_{LM}(\theta,\varphi) r^2\mathrm d r\sin\theta\mathrm d \theta\mathrm d \varphi=\delta_{L'L}\delta_{M'M}
> $$
>
> > 克罗内克记号
> > $$
> > \delta_{ab}=\begin{cases}1,\quad a=b\\0,\quad a\ne b\end{cases}
> > $$
> >
>
> 球谐函数有一个对我们来说很有用的性质：
> $$
> [\frac{1}{\sin\theta}\frac\partial{\partial\theta}\sin\theta\frac\partial{\partial\theta}+\frac 1 {\sin^2\theta}\frac{\partial^2}{\partial\varphi^2}]Y_{LM}(\theta,\varphi)=-L(L+1)Y_{LM}(\theta,\varphi)
> $$
> 称为本征值方程，即将中括号内的微商算符作用在球谐函数上，等于球谐函数乘以一个常数。

令
$$
\Phi(\vec r)=\Phi(r,\theta,\varphi)=R(r)Y_{LM}(\theta,\varphi)
$$
代回上面的方程中，得到
$$
\begin{align}
E\Phi(\vec r)&=ER(r)Y_{LM}(\theta,\varphi)\\
&=-\frac{h^2}{2m}\frac 1 {r^2}\frac{\partial }{\partial r}r^2\frac{\partial R(r)}{\partial r}Y_{LM}(\theta,\varphi)-\frac{h^2}{2mr^2}[\frac{1}{\sin\theta}\frac\partial{\partial\theta}\sin\theta\frac{\partial Y_{LM}}{\partial\theta }+\frac 1 {\sin^2\theta}\frac{\partial^2 Y_{LM}}{\partial\varphi^2}]R(r)-\frac{e^2}rR(r)Y_{LM}(\theta,\varphi)\\
&=-\frac{h^2}{2m}\frac 1 {r^2}\frac{\partial }{\partial r}r^2\frac{\partial R(r)}{\partial r}Y_{LM}(\theta,\varphi)-\frac{h^2}{2mr^2}[-L(L+1)Y_{LM}(\theta,\varphi)]R(r)-\frac{e^2}rR(r)Y_{LM}(\theta,\varphi)\\
\end{align}
$$
约去等式两边的球谐函数，得到常微分方程
$$
ER(r)=-\frac{h^2}{2m}\frac 1 {r^2}\frac{\mathrm d }{\mathrm d r}r^2\frac{\mathrm d R(r)}{\mathrm d r}-\frac{h^2}{2mr^2}[-L(L+1)]R(r)-\frac{e^2}rR(r)
$$
由于$R(r)$是与$L$有关的，所以我们写成角标的形式，即$R_L(r)$。观察这个方程的第一项，可以发现如果我们令$R_L(r)=\chi_L(r)/r$，有
$$
\frac 1 {r^2}\frac{\mathrm d }{\mathrm d r}r^2\frac{\mathrm d R_L(r)}{\mathrm d r}=\frac1r\chi_L^{\prime\prime}(r)
$$
那么方程可以进一步简化为
$$
E\frac{\chi_L(r)}{r}=-\frac{\hbar^2}{2m}\frac 1r\chi_L^{\prime\prime}(r)+\frac{\hbar^2L(L+1)}{2mr}\frac{\chi_L(r)}{r}-\frac{e^2}r\frac{\chi_L(r)}r\\
\chi_L^{\prime\prime}(r)+[\frac{2m}{\hbar^2}(E+\frac {e^2}r)-\frac{L(L+1)}{r^2}]\chi_L(r)=0
$$
解这个方程首先要做奇异点分析，显然这个方程的极点是在$r=0$和$r=\infty$。

- 当$r\rightarrow\infty$时，上式退化为
  $$
  \chi_L^{\prime\prime}(r)+\frac{2m}{\hbar^2}E\chi_L(r)=0
  $$
  可以解得
  $$
  \begin{cases}
  \chi_L^{(1)}(r)=\exp[-\sqrt{\frac{2mE}{\hbar^2}}r]\quad \checkmark\\
  \chi_L^{(2)}(r)=\exp[\sqrt{\frac{2mE}{\hbar^2}}r]\quad \times
  \end{cases}
  $$
  我们希望这个解在空间各点都是有限的，所以取第一个解。

- 当$r\rightarrow0$时，
  $$
  \chi_L^{\prime\prime}(r)-\frac{L(L+1)}{r^2}\chi_L(r)=0
  $$
  可以解得
  $$
  \begin{cases}
  \chi_L^{(a)}(r)=r^{L+1}\quad \checkmark\\
  \chi_L^{(b)}(r)=r^{-L}\quad \times
  \end{cases}
  $$
  同理去掉发散的解。

现在令
$$
\chi_L(r)=\chi_L^{(1)}(r)\chi_L^{(a)}(r)u_L(r)
$$
代回到薛定谔方程中，整理一下可以得到只与$u_L(r)$有关的微分方程：
$$
u_L^{\prime\prime}(r)r^{L+1}+\left(2(L+1)r^L-2r^{L+1}\sqrt{-\frac{2mE}{\hbar^2}}\right)u_L^\prime(r)-\left(2(L+1)r^L\sqrt{-\frac{2mE}{\hbar^2}}-\frac{2m}{\hbar^2}e^2r^L\right)u_L(r)=0
$$
在两边消去$r^L$并写成微分形式，得到
$$
r\frac{\mathrm d^2 u_L(r)}{\mathrm d r^2}+\left(2(L+1)-2r\sqrt{-\frac{2mE}{\hbar^2}}\right)\frac{\mathrm d u_L(r)}{\mathrm d r}-\left(2(L+1)\sqrt{-\frac{2mE}{\hbar^2}}-\frac{2m}{\hbar^2}e^2\right)u_L(r)=0
$$
在多数情况下，做到这一步就无法继续进行了，必须用计算机进行求解，但氢原子刚好很特殊，我们可以试图往合流超几何微分方程上凑。

> 合流超几何微分方程的标准形式是这样的：
> $$
> \xi\frac{\mathrm d^2u_L(\xi)}{\mathrm d \xi^2}+(\gamma-\xi)\frac{\mathrm du_L(\xi)}{\mathrm d\xi}-\alpha u_L(\xi)=0
> $$
> 其中$\gamma$和$\alpha$是常数。
>
> 在$\xi=0$处具有解析解：
> $$
> F(\alpha,\gamma,\xi)=1+\frac\alpha\gamma\xi+\frac1{2!}\frac{\alpha(\alpha+1)}{\gamma(\gamma+1)}\xi^2+\frac1{3!}\frac{\alpha(\alpha+1)(\alpha+2)}{\gamma(\gamma+1)(\gamma+2)}\xi^3+\dots
> $$
>

令$2r\sqrt{-2mE/\hbar^2}=\xi$，则
$$
\frac{\mathrm d u}{\mathrm d r}=\frac{\mathrm d u}{\mathrm d \xi}\frac{\mathrm d \xi}{\mathrm d r}=2\sqrt{-\frac{2mE}{\hbar^2}}\frac{\mathrm d u}{\mathrm d \xi}\\
\frac{\mathrm d^2u}{\mathrm dr^2}=(2\sqrt{-\frac{2mE}{\hbar^2}})^2\frac{\mathrm d^2u}{\mathrm d \xi^2}
$$
上式可以化为
$$
\xi\frac{\mathrm d^2u_L(\xi)}{\mathrm d\xi^2}+(2(L+1)-\xi)\frac{\mathrm du_L(\xi)}{\mathrm d\xi}-\frac{(2(L+1)\sqrt{-\frac{2mE}{\hbar^2}}-\frac{2m}{\hbar^2}e^2)}{2\sqrt{-\frac{2mE}{\hbar^2}}}u_L(\xi)=0
$$
与标准合流超几何方程比较很容易就可以写出它的解析解，但我们注意到这个解是一个发散的无穷级数，为了得到收敛的结果，我们要想办法把这个无穷级数截断成一个多项式。

观察解的形式我们可以发现，如果令$\alpha=0$，则解会被截断成一项：$F=1$；如果令$\alpha=-1$，则解会被截断成前两项。

那么我么令$\alpha=-n_r,\quad n_r=1,2,3\dots$，就可以完成截断
$$
\alpha=\frac{(2(L+1)\sqrt{-\frac{2mE}{\hbar^2}}-\frac{2m}{\hbar^2}e^2)}{2\sqrt{-\frac{2mE}{\hbar^2}}}=-n_r
$$
化简得到
$$
E=-\frac{me^4}{2\hbar^2(L+1+n_r)^2}
$$
显而易见，只要令$n=L+1+n_r$，就得到了氢原子能级公式
$$
E=-\frac{2\pi^2me^4}{n^2h^2}
$$
常数项的这一差异解释了氢原子光谱的谱线亮度问题。对于一个给定的n，所有
$$
L=0,1,2,\dots,n-1\\
n_r=n-1,n-2,\dots,0
$$
的状态具有相同的能量，这种现象称为简并。在$Y_{LM}$中，$L\le M\le L$，有2L+1个M，氢原子每个状态的简并度
$$
N_n=\sum_{L=0}^{n-1}(2L+1)=2\sum_{L=0}^{n-1}L+n=2\times\frac{n(n-1)}{2}+n=n^2
$$
简并度越高，这条谱线的亮度就越亮。

最后我们给出氢原子的波函数
$$
\psi(\vec r,t)\approx \frac1r\exp(-\frac\xi2)r^{L+1}F(-n_r,2(L+1),\xi)Y_{LM}(\theta,\varphi)\exp(-\frac{iEt}\hbar), \xi=2r\sqrt{-\frac{2m}{\hbar^2}E}
$$

### 1.6 波函数的几率解释

对于薛定谔来讲，一个更为迫切的任务是如何解释波函数的物理意义。

对于波函数
$$
i\hbar\frac{\partial}{\partial t}\psi=-\frac{\hbar^2}{2m}\nabla^2\psi+V(r)\psi\tag1
$$
将方程左乘$\psi^*(r)$，得到
$$
i\hbar\psi^*(r)\frac\partial{\partial t}\psi(r)=-\frac{\hbar^2}{2m}\psi^*(r)\nabla^2\psi(r)+\psi^*(r)V(r)\psi(r)\tag2
$$
对（1）取复共轭
$$
-i\hbar\frac{\partial}{\partial t}\psi^*=-\frac{\hbar^2}{2m}\nabla^2\psi^*+V(r)\psi^*\tag3
$$
将（3）再左乘$\psi$
$$
-i\hbar\psi\frac{\partial}{\partial t}\psi^*=-\frac{\hbar^2}{2m}\psi\nabla^2\psi^*+V(r)\psi\psi^*\tag4
$$
（2）-（4），
$$
\begin{align}i\hbar(\psi^*\frac{\partial \psi}{\partial t}+\psi\frac{\partial \psi^*}{\partial t})&=-\frac{\hbar^2}{2m}(\psi^*\nabla^2\psi-\psi\nabla^2\psi^*)\\i\hbar\frac{\partial}{\partial t}(\psi^*\psi)&=-\frac{\hbar^2}{2m}\nabla(\psi\nabla\psi^*-\psi^*\nabla\psi)\end{align}\\
\frac\partial{\partial t}(\psi^*\psi)+\frac{\hbar}{2mi}\nabla(\psi\nabla\psi^*-\psi^*\nabla\psi)=0
$$
薛定谔注意到$\psi^*\psi=|\psi|^2\ge 0$，这与流体力学中的连续性方程很像：
$$
\frac{\partial\rho(\vec r,t)}{\partial t}+\nabla\cdot\vec J=0, \rho(\vec r,t)\ge 0
$$
那么令$\rho=\psi^*\psi$，表示某种密度，$J=(\hbar/2mi)(\psi\nabla\psi^*-\psi^*\nabla\psi)$，表示某种流。

很自然的，薛定谔认为这是电子的密度和电子的质量流。但是很快人们就发现这样的解释有很多问题，因为一般的波函数都是与时间有关的，这就意味着电子在经历了一段时间后会在空间中很大的区域内非零，即电子越来越大了，这显然是不现实的。

> 最后，波恩（Born）提出的几率解释克服了这一困难。他也因此获得了1954年的诺贝尔奖。Born在量子力学的建立中参与了二人文章和三人文章，做了不小的贡献，但最后只有海森堡一人得了诺贝尔奖，海森堡也为这件事很愧疚，一方面波恩是他的老师，另一方面他也承认波恩确实起了很重要的作用。1954年波恩因为几率解释得奖之后，海森堡写信给波恩，表示心终于沉下来了。
>
> 几率解释是十分重要的，因为在给出一个正确的解释之后，所有之后的事情都得到了顺利的进行。

Born提出，考虑单个电子的话，$\rho(\vec r ,t)=|\psi(\vec r,t)|^2$代表在时刻t，在以r为中心的一个小区域中找到该电子的几率密度。电子可以出现在空间的不同区域内，但是一旦出现就是一个整体，具有固定的电荷和质量等属性。

另一方面，如果考虑N各个处于相同状态的粒子，可以将$N|\psi(\vec r ,t )|$解释为时刻t时，在空间r处的粒子密度，而将$Nq|\psi(\vec r,t)|^2$解释为电荷密度。

我们很自然的要求
$$
\int_\Omega |\psi(\vec r, t)|^2\mathrm d \vec r = 1 < \infty
$$
定义平方可积空间
$$
L^2(\Omega)=\{\psi|\int_\Omega|\psi|^2\mathrm d r=A\}
$$
这一空间也称为希尔伯特（Hilbert）空间，是线性的，也就是说对数乘和加法是封闭的。

$\psi(\vec r,t)$被称为几率幅，它不是一个可观测的量，因此可以被写作
$$
\psi(\vec r, t)=|\psi(\vec r ,t)|e^{i\alpha(\vec r,t)}
$$
其中$\exp(i\alpha)$称为相位，若两个波函数仅有相位之差，则他们在物理上是等价的。

### 1.7 Heisenberg的测不准原理

> 薛定谔给出了证明，波动力学和矩阵力学是完全等价的（过程暂略）。这让海森堡十分不爽，应为海森堡花了至少五年的时间~~，还进行了很多哲学思考~~，然后被两个人不经意间搞出一个等价的东西，然后海森堡就想多做一些东西。
> 
> 1927年，海森堡引入了测不准原理。

对易关系中，两个物理量不对易的物理意义是什么呢？也就是说，假设有
$$
[\hat A ,\hat B]=i\hat C\ne 0
$$
我们取一个允许态$\psi(\vec r,t)$。定义
$$
\bar A =(\psi , \hat A\psi)=\int_\Omega \mathrm d \vec r \psi^*(\vec r,t)\hat A\psi(\vec r,t)\\
\bar B =(\psi , \hat A\psi) = \int_\Omega \mathrm d \vec r \psi^*(\vec r,t)\hat B\psi(\vec r,t)
$$
海森堡证明了如下的关系：
$$
\overline{(\hat A -\bar A)^2}\cdot\overline{(\hat B - \bar B)^2} \ge \frac 1 4 \bar C ^2
$$
称为海森堡测不准原理的表达式。（证明过程暂略）

