### 032补充

积分定理间的关系

从微积分基本定理, 到梯度定理, 再到格林定理, 以及高斯 (散度) 定理, 和斯托克斯 (旋度) 定理, 它们的味道似乎都有点相似, 尤其时最后三者, 用比较微分几何一点的语言来说, 都是: 若有一个微分形式 $$\omega$$ , $$S$$ 是一个流形 (其维度大于 $$\omega$$ 的阶数), 这个流形的表面记作 $$\partial S$$, 那么
$$
\int_S\mathrm{d}\omega=\int_{\partial S}\omega,
$$
也就是前面提过一次的广义斯托克斯定理. 当然, 这是比较"天上"的表述, 接地气一点, 我们来一点一点看一下各定理是怎么联系起来的.

首先要正式的介绍一下楔积或者外积了, 这个概念在【026】中已经简单提到过, 它满足以下运算法则:

- 对数乘交换: $$a(\mathrm{d}x\wedge\mathrm{d}y)=(a\mathrm{d}x)\wedge\mathrm{d}y=\mathrm{d}x\wedge(a\mathrm{d}y)$$
- 加法分配律: $$\mathrm{d}x\wedge(\mathrm{d}y\wedge\mathrm{d}z)=\mathrm{d}x\wedge\mathrm{d}y+\mathrm{d}x\wedge\mathrm{d}z$$
- 反交换律: $$\mathrm{d}x\wedge\mathrm{d}y=-\mathrm{d}y\wedge\mathrm{d}x$$
- 结合律: $$\mathrm{d}x\wedge(\mathrm{d}y\wedge\mathrm{d}z)=(\mathrm{d}x\wedge\mathrm{d}y)\wedge\mathrm{d}z$$

然后便有外微分形式, 可以简单粗暴地将其理解为一个等待被积分的对象. 形如 $$f(x,y,z)$$ 的标量场, 便可视作0阶外微分形式; 形如 $$f(x,y,z)\mathrm{d}x$$ 的便是1阶外微分形式; 形如 $$f(x,y,z)\mathrm{d}x\wedge\mathrm{d}y$$ 的便是2阶外微分形式... and so on. 

如此这般, 前面的一系列定理便可更整洁地被写作:

Let $$\omega=P\mathrm{d}x-Q\mathrm{d}y$$, 格林定理:
$$
\int\omega=\iint\mathrm{d}\omega.
$$
即原本的: $$\int P\mathrm{d}x-Q\mathrm{d}y=\iint\left(-\frac{\partial P}{\partial y}+\frac{\partial Q}{\partial x}\right)|\mathrm{d}x\wedge\mathrm{d}y|$$.

类似得, let $$\omega=P\mathrm{d}x\wedge\mathrm{d}y+Q\mathrm{d}z\wedge\mathrm{d}x+R\mathrm{d}z\wedge\mathrm{d}y$$

https://www.cnblogs.com/jiangongyuxiao/p/15088081.html













