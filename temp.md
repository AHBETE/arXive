## 量子主方程速通 (Master equation - Lindblad form)

### 传统方法的不足

省略一些篇幅和计算, 大致的思想是: 如果考虑一个带阻尼的谐振子 (damped harmonic oscillator), 根据它位置和动量算符的对易子 (commutator) 得到它位置和动量的不确定关系, 这一项会是指数衰减的; 这显然是不正确的, 因此需要一个新的方法来处理能量 (或者信息) 有耗散 (dissipation) 的量子系统.

### 系统 + 环境 (热库) 法

把系统和环境都粗暴地视作谐振子, 系统的升降算符记作 $$\hat{a}$$ 和 $$\hat{a}^\dagger$$, 环境的升降算符记作 $$\hat{b}$$ 和 $$\hat{b}^\dagger$$. 在旋波近似下, 系统和环境整体的哈密顿算符是:
$$
\hat{H}=\hbar\omega\hat{a}^\dagger\hat{a}+\hbar\omega\hat{b}^\dagger\hat{b}+\hbar\kappa(\hat{a}^\dagger\hat{b}+\hat{a}\hat{b}^\dagger).
$$

> 前两项 $$\hat{升}\hat{降}$$ 这样的形式会读出系统/环境的光子 (photon) 或声子 (phonon) 数, 乘上频率和普朗克常数便是系统/环境的能量, 最后一项是环境和系统的"交互 (interaction) 项", $$\kappa$$ 是系统和环境的耦合常数 (交互得强度, 是否容易发生能量交换);
>
> 旋波近似前完整的项应该还包括$$\hat{a}^\dagger\hat{b}^\dagger$$ 和 $$\hat{a}\hat{b}$$, 这一近似有两种解释:
> (i) 只保留能量守恒项, 两个都是升算符表示环境和系统能量同时提升, 两个都是降算符表示环境和系统能量同时下降, 在经典上是不合理的 (但是因为能量和时间的对易关系, 实际上在很短的的时间内, 这样的事件是可以发生的, 但是概率上很小, 所以忽略);
> (ii) 算符作用到系统/环境上时, 将系统和环境的频率分别记作 $$\omega_a$$ 和 $$\omega_b$$, 同时升或者同时讲的算符会导致 $$\mathrm{e}^{i(\omega_a+\omega_b)}$$ 和 $$\mathrm{e}^{i(-\omega_a-\omega_b)}$$ 项的出现, 相比于一升一降的$$\mathrm{e}^{\pm i(\omega_a-\omega_b)}$$, 前二者是快速振荡的, 在后二者 (which 是我们更关注的对象) 变化的时间尺度上, 前者的变化就被"平均"掉了.

利用位置 - 动量表征, 