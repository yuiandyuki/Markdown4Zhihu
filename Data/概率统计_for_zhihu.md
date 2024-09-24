本文记载《Introduction to Mathematical Statistics and Its Applications》这本书的各种定义定理

## Ch7 : Inferences based on the normal distribution

### Theorem 7.3.1

设  <img src="https://www.zhihu.com/equation?tex=U = \sum_{j=1}^{m} Z_j^2" alt="U = \sum_{j=1}^{m} Z_j^2" class="ee_img tr_noresize" eeimg="1"> ，其中  <img src="https://www.zhihu.com/equation?tex=Z_1, Z_2, ..., Z_m" alt="Z_1, Z_2, ..., Z_m" class="ee_img tr_noresize" eeimg="1">  是独立的标准正态随机变量。则  <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1">  服从参数  <img src="https://www.zhihu.com/equation?tex=r = \frac{m}{2}" alt="r = \frac{m}{2}" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=\lambda = \frac{1}{2}" alt="\lambda = \frac{1}{2}" class="ee_img tr_noresize" eeimg="1">  的伽马分布，即：


<img src="https://www.zhihu.com/equation?tex=f_U(u) = \frac{1}{2^{m/2} \Gamma \left( \frac{m}{2} \right)} u^{(m/2)-1} e^{-u/2}, \quad u \geq 0" alt="f_U(u) = \frac{1}{2^{m/2} \Gamma \left( \frac{m}{2} \right)} u^{(m/2)-1} e^{-u/2}, \quad u \geq 0" class="ee_img tr_noresize" eeimg="1">

推导过程如下：

首先，取  <img src="https://www.zhihu.com/equation?tex=m = 1" alt="m = 1" class="ee_img tr_noresize" eeimg="1"> 。对任意  <img src="https://www.zhihu.com/equation?tex=u \geq 0" alt="u \geq 0" class="ee_img tr_noresize" eeimg="1"> ，我们计算：


<img src="https://www.zhihu.com/equation?tex=F_{Z^2}(u) = P(Z^2 \leq u) = P(-\sqrt{u} \leq Z \leq \sqrt{u}) = 2P(0 \leq Z \leq \sqrt{u})" alt="F_{Z^2}(u) = P(Z^2 \leq u) = P(-\sqrt{u} \leq Z \leq \sqrt{u}) = 2P(0 \leq Z \leq \sqrt{u})" class="ee_img tr_noresize" eeimg="1">

通过计算积分可以得到  <img src="https://www.zhihu.com/equation?tex=F_{Z^2}(u)" alt="F_{Z^2}(u)" class="ee_img tr_noresize" eeimg="1">  的值。然后，对其求导，得到  <img src="https://www.zhihu.com/equation?tex=f_{Z^2}(u)" alt="f_{Z^2}(u)" class="ee_img tr_noresize" eeimg="1"> ：


<img src="https://www.zhihu.com/equation?tex=f_{Z^2}(u) = \frac{1}{\sqrt{2\pi}} \frac{1}{2\sqrt{u}} e^{-u/2} = \frac{1}{2^{1/2} \Gamma(1/2)} u^{(1/2)-1} e^{-u/2}" alt="f_{Z^2}(u) = \frac{1}{\sqrt{2\pi}} \frac{1}{2\sqrt{u}} e^{-u/2} = \frac{1}{2^{1/2} \Gamma(1/2)} u^{(1/2)-1} e^{-u/2}" class="ee_img tr_noresize" eeimg="1">

可以看到，这与伽马分布的形式一致，参数  <img src="https://www.zhihu.com/equation?tex=r = \frac{1}{2}" alt="r = \frac{1}{2}" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=\lambda = \frac{1}{2}" alt="\lambda = \frac{1}{2}" class="ee_img tr_noresize" eeimg="1"> 。

通过定理4.6.4，总结  <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1">  个此类平方的和具有上述伽马分布形式，参数为  <img src="https://www.zhihu.com/equation?tex=r = \frac{m}{2}" alt="r = \frac{m}{2}" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=\lambda = \frac{1}{2}" alt="\lambda = \frac{1}{2}" class="ee_img tr_noresize" eeimg="1"> 。


### Definition 7.3.1

设  <img src="https://www.zhihu.com/equation?tex=U = \sum_{j=1}^{m} Z_j^2" alt="U = \sum_{j=1}^{m} Z_j^2" class="ee_img tr_noresize" eeimg="1"> ，其中  <img src="https://www.zhihu.com/equation?tex=Z_1, Z_2, \dots, Z_m" alt="Z_1, Z_2, \dots, Z_m" class="ee_img tr_noresize" eeimg="1">  是独立的标准正态随机变量，那么  <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1">  的概率密度函数称为具有  <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1">  个自由度的**卡方分布**。

### Theorem 7.3.2

设  <img src="https://www.zhihu.com/equation?tex=Y_1, Y_2, \dots, Y_n" alt="Y_1, Y_2, \dots, Y_n" class="ee_img tr_noresize" eeimg="1">  是从均值为  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1">  且方差为  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1">  的正态分布中抽取的随机样本。则：

a.  <img src="https://www.zhihu.com/equation?tex=S^2" alt="S^2" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=\overline{Y}" alt="\overline{Y}" class="ee_img tr_noresize" eeimg="1">  是相互独立的。

b.  <img src="https://www.zhihu.com/equation?tex=\frac{(n-1)S^2}{\sigma^2} = \frac{1}{\sigma^2} \sum_{i=1}^{n}(Y_i - \overline{Y})^2" alt="\frac{(n-1)S^2}{\sigma^2} = \frac{1}{\sigma^2} \sum_{i=1}^{n}(Y_i - \overline{Y})^2" class="ee_img tr_noresize" eeimg="1">  服从具有  <img src="https://www.zhihu.com/equation?tex=n - 1" alt="n - 1" class="ee_img tr_noresize" eeimg="1">  个自由度的卡方分布。

证明在附录

### Definition 7.3.2

假设  <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=V" alt="V" class="ee_img tr_noresize" eeimg="1">  是具有  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1">  个自由度的独立卡方随机变量。形式为  <img src="https://www.zhihu.com/equation?tex=\frac{V/m}{U/n}" alt="\frac{V/m}{U/n}" class="ee_img tr_noresize" eeimg="1">  的随机变量称为具有  <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  个自由度的 **F 分布**。

### Theorem 7.3.3

假设  <img src="https://www.zhihu.com/equation?tex=F_{m,n} = \frac{V/m}{U/n}" alt="F_{m,n} = \frac{V/m}{U/n}" class="ee_img tr_noresize" eeimg="1">  表示具有  <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  个自由度的 F 分布随机变量。则  <img src="https://www.zhihu.com/equation?tex=F_{m,n}" alt="F_{m,n}" class="ee_img tr_noresize" eeimg="1">  的概率密度函数为：


<img src="https://www.zhihu.com/equation?tex=f_{F_{m,n}}(w) = \frac{\Gamma \left( \frac{m+n}{2} \right) m^{m/2} n^{n/2} w^{(m/2)-1}}{\Gamma \left( \frac{m}{2} \right) \Gamma \left( \frac{n}{2} \right) (n+mw)^{(m+n)/2}}, \quad w \geq 0" alt="f_{F_{m,n}}(w) = \frac{\Gamma \left( \frac{m+n}{2} \right) m^{m/2} n^{n/2} w^{(m/2)-1}}{\Gamma \left( \frac{m}{2} \right) \Gamma \left( \frac{n}{2} \right) (n+mw)^{(m+n)/2}}, \quad w \geq 0" class="ee_img tr_noresize" eeimg="1">

我们从  <img src="https://www.zhihu.com/equation?tex=V/U" alt="V/U" class="ee_img tr_noresize" eeimg="1">  的概率密度函数开始推导。根据定理 7.3.1，我们知道：


<img src="https://www.zhihu.com/equation?tex=f_V(v) = \frac{1}{2^{m/2} \Gamma(m/2)} v^{(m/2)-1} e^{-v/2}, \quad f_U(u) = \frac{1}{2^{n/2} \Gamma(n/2)} u^{(n/2)-1} e^{-u/2}" alt="f_V(v) = \frac{1}{2^{m/2} \Gamma(m/2)} v^{(m/2)-1} e^{-v/2}, \quad f_U(u) = \frac{1}{2^{n/2} \Gamma(n/2)} u^{(n/2)-1} e^{-u/2}" class="ee_img tr_noresize" eeimg="1">

通过使用定理 3.8.4，我们可以计算  <img src="https://www.zhihu.com/equation?tex=W = \frac{V}{U}" alt="W = \frac{V}{U}" class="ee_img tr_noresize" eeimg="1">  的概率密度函数  <img src="https://www.zhihu.com/equation?tex=f_{V/U}(w)" alt="f_{V/U}(w)" class="ee_img tr_noresize" eeimg="1"> ：


<img src="https://www.zhihu.com/equation?tex=f_{V/U}(w) = \int_0^\infty |u| f_U(u) f_V(uw) du" alt="f_{V/U}(w) = \int_0^\infty |u| f_U(u) f_V(uw) du" class="ee_img tr_noresize" eeimg="1">

将  <img src="https://www.zhihu.com/equation?tex=f_U(u)" alt="f_U(u)" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=f_V(uw)" alt="f_V(uw)" class="ee_img tr_noresize" eeimg="1">  代入上述积分中，得出：


<img src="https://www.zhihu.com/equation?tex=f_{V/U}(w) = \frac{1}{2^{(n+m)/2} \Gamma(n/2) \Gamma(m/2)} w^{(m/2)-1} \int_0^\infty u^{n/2 + m/2 - 1} e^{-(1+w)u/2} du" alt="f_{V/U}(w) = \frac{1}{2^{(n+m)/2} \Gamma(n/2) \Gamma(m/2)} w^{(m/2)-1} \int_0^\infty u^{n/2 + m/2 - 1} e^{-(1+w)u/2} du" class="ee_img tr_noresize" eeimg="1">

这个积分是伽马分布的积分部分，最终我们得到：


<img src="https://www.zhihu.com/equation?tex=f_{V/U}(w) = \frac{1}{2^{(n+m)/2} \Gamma(n/2) \Gamma(m/2)} w^{(m/2)-1} \frac{\Gamma \left( \frac{n+m}{2} \right)}{(1+w)^{(n+m)/2}}" alt="f_{V/U}(w) = \frac{1}{2^{(n+m)/2} \Gamma(n/2) \Gamma(m/2)} w^{(m/2)-1} \frac{\Gamma \left( \frac{n+m}{2} \right)}{(1+w)^{(n+m)/2}}" class="ee_img tr_noresize" eeimg="1">

最终，F 分布的概率密度函数  <img src="https://www.zhihu.com/equation?tex=f_{F_{m,n}}(w)" alt="f_{F_{m,n}}(w)" class="ee_img tr_noresize" eeimg="1">  为：


<img src="https://www.zhihu.com/equation?tex=f_{F_{m,n}}(w) = \frac{\Gamma \left( \frac{m+n}{2} \right) m^{m/2} n^{n/2} w^{(m/2)-1}}{\Gamma \left( \frac{m}{2} \right) \Gamma \left( \frac{n}{2} \right) (n+mw)^{(m+n)/2}}" alt="f_{F_{m,n}}(w) = \frac{\Gamma \left( \frac{m+n}{2} \right) m^{m/2} n^{n/2} w^{(m/2)-1}}{\Gamma \left( \frac{m}{2} \right) \Gamma \left( \frac{n}{2} \right) (n+mw)^{(m+n)/2}}" class="ee_img tr_noresize" eeimg="1">

### Definition 7.3.3

设  <img src="https://www.zhihu.com/equation?tex=Z" alt="Z" class="ee_img tr_noresize" eeimg="1">  为标准正态随机变量， <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1">  为与  <img src="https://www.zhihu.com/equation?tex=Z" alt="Z" class="ee_img tr_noresize" eeimg="1">  独立的卡方随机变量，自由度为  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 。具有  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  个自由度的 **Student t 比值** 记作  <img src="https://www.zhihu.com/equation?tex=T_n" alt="T_n" class="ee_img tr_noresize" eeimg="1"> ，其定义为：


<img src="https://www.zhihu.com/equation?tex=T_n = \frac{Z}{\sqrt{U/n}}" alt="T_n = \frac{Z}{\sqrt{U/n}}" class="ee_img tr_noresize" eeimg="1">


### lemma

 <img src="https://www.zhihu.com/equation?tex=T_n" alt="T_n" class="ee_img tr_noresize" eeimg="1">  的概率密度函数是对称的，即  <img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = f_{T_n}(-t)" alt="f_{T_n}(t) = f_{T_n}(-t)" class="ee_img tr_noresize" eeimg="1"> ，对所有  <img src="https://www.zhihu.com/equation?tex=t" alt="t" class="ee_img tr_noresize" eeimg="1">  都成立。

**证明**：

为方便记号，设  <img src="https://www.zhihu.com/equation?tex=V = \sqrt{\frac{U}{n}}" alt="V = \sqrt{\frac{U}{n}}" class="ee_img tr_noresize" eeimg="1"> 。根据定理 3.8.4 和  <img src="https://www.zhihu.com/equation?tex=Z" alt="Z" class="ee_img tr_noresize" eeimg="1">  的概率密度函数的对称性，有：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = \int_0^\infty v f_V(v) f_Z(tv) dv = \int_0^\infty v f_V(v) f_Z(-tv) dv = f_{T_n}(-t)" alt="f_{T_n}(t) = \int_0^\infty v f_V(v) f_Z(tv) dv = \int_0^\infty v f_V(v) f_Z(-tv) dv = f_{T_n}(-t)" class="ee_img tr_noresize" eeimg="1">

因此， <img src="https://www.zhihu.com/equation?tex=T_n" alt="T_n" class="ee_img tr_noresize" eeimg="1">  的概率密度函数  <img src="https://www.zhihu.com/equation?tex=f_{T_n}(t)" alt="f_{T_n}(t)" class="ee_img tr_noresize" eeimg="1">  是对称的。

### Theorem 7.3.4

具有  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  个自由度的 **Student t** 随机变量的概率密度函数为：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = \frac{\Gamma \left( \frac{n+1}{2} \right)}{\sqrt{n\pi} \Gamma \left( \frac{n}{2} \right)} \left( 1 + \frac{t^2}{n} \right)^{-\frac{n+1}{2}}, \quad -\infty < t < \infty" alt="f_{T_n}(t) = \frac{\Gamma \left( \frac{n+1}{2} \right)}{\sqrt{n\pi} \Gamma \left( \frac{n}{2} \right)} \left( 1 + \frac{t^2}{n} \right)^{-\frac{n+1}{2}}, \quad -\infty < t < \infty" class="ee_img tr_noresize" eeimg="1">

**证明**：

1. 首先，注意到  <img src="https://www.zhihu.com/equation?tex=T_n^2 = \frac{Z^2}{U/n}" alt="T_n^2 = \frac{Z^2}{U/n}" class="ee_img tr_noresize" eeimg="1">  具有  <img src="https://www.zhihu.com/equation?tex=1" alt="1" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">  个自由度的 F 分布。因此， <img src="https://www.zhihu.com/equation?tex=f_{T_n^2}(t^2)" alt="f_{T_n^2}(t^2)" class="ee_img tr_noresize" eeimg="1">  可以表示为：


<img src="https://www.zhihu.com/equation?tex=f_{T_n^2}(t^2) = \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{n}{2} \right)} t^{-1/2} \frac{1}{(n+t)^{(n+1)/2}}, \quad t > 0" alt="f_{T_n^2}(t^2) = \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{n}{2} \right)} t^{-1/2} \frac{1}{(n+t)^{(n+1)/2}}, \quad t > 0" class="ee_img tr_noresize" eeimg="1">

2. 设  <img src="https://www.zhihu.com/equation?tex=t > 0" alt="t > 0" class="ee_img tr_noresize" eeimg="1"> 。根据  <img src="https://www.zhihu.com/equation?tex=f_{T_n}(t)" alt="f_{T_n}(t)" class="ee_img tr_noresize" eeimg="1">  的对称性，我们有：


<img src="https://www.zhihu.com/equation?tex=F_{T_n}(t) = P(T_n \leq t) = \frac{1}{2} + P(0 \leq T_n \leq t)" alt="F_{T_n}(t) = P(T_n \leq t) = \frac{1}{2} + P(0 \leq T_n \leq t)" class="ee_img tr_noresize" eeimg="1">

3. 接着，我们通过对称性展开如下：


<img src="https://www.zhihu.com/equation?tex=F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} P(-t \leq T_n \leq t) = \frac{1}{2} + \frac{1}{2} P(0 \leq T_n \leq t)" alt="F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} P(-t \leq T_n \leq t) = \frac{1}{2} + \frac{1}{2} P(0 \leq T_n \leq t)" class="ee_img tr_noresize" eeimg="1">

4. 再将其写为：


<img src="https://www.zhihu.com/equation?tex=F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} P(0 \leq T_n^2 \leq t^2)" alt="F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} P(0 \leq T_n^2 \leq t^2)" class="ee_img tr_noresize" eeimg="1">

5. 于是可以得到：


<img src="https://www.zhihu.com/equation?tex=F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} F_{T_n^2}(t^2)" alt="F_{T_n}(t) = \frac{1}{2} + \frac{1}{2} F_{T_n^2}(t^2)" class="ee_img tr_noresize" eeimg="1">

6. 对  <img src="https://www.zhihu.com/equation?tex=F_{T_n}(t)" alt="F_{T_n}(t)" class="ee_img tr_noresize" eeimg="1">  求导，我们得到：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = \frac{d}{dt} F_{T_n}(t) = t \cdot f_{T_n^2}(t^2)" alt="f_{T_n}(t) = \frac{d}{dt} F_{T_n}(t) = t \cdot f_{T_n^2}(t^2)" class="ee_img tr_noresize" eeimg="1">

7.  <img src="https://www.zhihu.com/equation?tex=f_{T_n}(t)" alt="f_{T_n}(t)" class="ee_img tr_noresize" eeimg="1">  的表达式进一步展开为：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = t \cdot \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{n}{2} \right)} (t^2)^{-1/2} \frac{1}{(n+t^2)^{(n+1)/2}}" alt="f_{T_n}(t) = t \cdot \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{n}{2} \right)} (t^2)^{-1/2} \frac{1}{(n+t^2)^{(n+1)/2}}" class="ee_img tr_noresize" eeimg="1">

8. 化简上式：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\sqrt{\pi} \Gamma \left( \frac{n}{2} \right)} \frac{1}{(n+t^2)^{(n+1)/2}}" alt="f_{T_n}(t) = \frac{n^{n/2} \Gamma \left( \frac{n+1}{2} \right)}{\sqrt{\pi} \Gamma \left( \frac{n}{2} \right)} \frac{1}{(n+t^2)^{(n+1)/2}}" class="ee_img tr_noresize" eeimg="1">

9. 最后得到  <img src="https://www.zhihu.com/equation?tex=T_n" alt="T_n" class="ee_img tr_noresize" eeimg="1">  的概率密度函数为：


<img src="https://www.zhihu.com/equation?tex=f_{T_n}(t) = \frac{\Gamma \left( \frac{n+1}{2} \right)}{\sqrt{n\pi} \Gamma \left( \frac{n}{2} \right)} \left( 1 + \frac{t^2}{n} \right)^{-\frac{n+1}{2}}" alt="f_{T_n}(t) = \frac{\Gamma \left( \frac{n+1}{2} \right)}{\sqrt{n\pi} \Gamma \left( \frac{n}{2} \right)} \left( 1 + \frac{t^2}{n} \right)^{-\frac{n+1}{2}}" class="ee_img tr_noresize" eeimg="1">


### Theorem 7.3.5

设  <img src="https://www.zhihu.com/equation?tex=Y_1, Y_2, \dots, Y_n" alt="Y_1, Y_2, \dots, Y_n" class="ee_img tr_noresize" eeimg="1">  是从均值为  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1">  且标准差为  <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1">  的正态分布中抽取的随机样本。那么


<img src="https://www.zhihu.com/equation?tex=T_{n-1} = \frac{\overline{Y} - \mu}{S / \sqrt{n}}" alt="T_{n-1} = \frac{\overline{Y} - \mu}{S / \sqrt{n}}" class="ee_img tr_noresize" eeimg="1">

服从自由度为  <img src="https://www.zhihu.com/equation?tex=n - 1" alt="n - 1" class="ee_img tr_noresize" eeimg="1">  的 **Student t** 分布。

**证明**：

我们可以将  <img src="https://www.zhihu.com/equation?tex=\frac{\overline{Y} - \mu}{S / \sqrt{n}}" alt="\frac{\overline{Y} - \mu}{S / \sqrt{n}}" class="ee_img tr_noresize" eeimg="1">  写成以下形式：


<img src="https://www.zhihu.com/equation?tex=\frac{\overline{Y} - \mu}{S / \sqrt{n}} = \frac{\overline{Y} - \mu}{\sigma / \sqrt{n}} \cdot \frac{1}{\sqrt{\frac{(n-1)S^2}{\sigma^2 (n-1)}}}" alt="\frac{\overline{Y} - \mu}{S / \sqrt{n}} = \frac{\overline{Y} - \mu}{\sigma / \sqrt{n}} \cdot \frac{1}{\sqrt{\frac{(n-1)S^2}{\sigma^2 (n-1)}}}" class="ee_img tr_noresize" eeimg="1">

其中  <img src="https://www.zhihu.com/equation?tex=\frac{\overline{Y} - \mu}{\sigma / \sqrt{n}}" alt="\frac{\overline{Y} - \mu}{\sigma / \sqrt{n}}" class="ee_img tr_noresize" eeimg="1">  是标准正态随机变量，且  <img src="https://www.zhihu.com/equation?tex=\frac{(n-1)S^2}{\sigma^2}" alt="\frac{(n-1)S^2}{\sigma^2}" class="ee_img tr_noresize" eeimg="1">  服从自由度为  <img src="https://www.zhihu.com/equation?tex=n - 1" alt="n - 1" class="ee_img tr_noresize" eeimg="1">  的卡方分布。

此外，定理 7.3.2 表明  <img src="https://www.zhihu.com/equation?tex=\frac{\overline{Y} - \mu}{\sigma / \sqrt{n}}" alt="\frac{\overline{Y} - \mu}{\sigma / \sqrt{n}}" class="ee_img tr_noresize" eeimg="1">  和  <img src="https://www.zhihu.com/equation?tex=\frac{(n-1)S^2}{\sigma^2}" alt="\frac{(n-1)S^2}{\sigma^2}" class="ee_img tr_noresize" eeimg="1">  彼此独立。

因此，根据定义 7.3.3， <img src="https://www.zhihu.com/equation?tex=\frac{\overline{Y} - \mu}{S / \sqrt{n}}" alt="\frac{\overline{Y} - \mu}{S / \sqrt{n}}" class="ee_img tr_noresize" eeimg="1">  服从自由度为  <img src="https://www.zhihu.com/equation?tex=n - 1" alt="n - 1" class="ee_img tr_noresize" eeimg="1">  的 **Student t** 分布。

