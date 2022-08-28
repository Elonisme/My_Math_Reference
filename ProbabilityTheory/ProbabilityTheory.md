<div class="cover" style="page-break-after:always;font-family:方正公文仿宋;width:100%;height:100%;border:none;margin: 0 auto;text-align:center;">
    <div style="width:60%;margin: 0 auto;height:0;padding-bottom:10%;">
        </br>
        <img src="https://upload.wikimedia.org/wikipedia/zh/thumb/5/58/Xihua_University_logo2.svg/220px-Xihua_University_logo2.svg.png" alt="校名" style="width:60%;"/>
    </div>
    </br></br></br></br></br>
    <div style="width:60%;margin: 0 auto;height:0;padding-bottom:40%;">
        <img src="https://upload.wikimedia.org/wikipedia/zh/thumb/2/23/Xihua_University_logo1.svg/200px-Xihua_University_logo1.svg.png" alt="校徽" style="width:50%;"/>
	</div>
    </br></br></br></br></br></br></br></br>
    <span style="font-family:华文黑体Bold;text-align:center;font-size:20pt;margin: 10pt auto;line-height:30pt;">《概率论》</span>
    <p style="text-align:center;font-size:14pt;margin: 0 auto">讲义 </p>
    </br>
    </br>
    <table style="border:none;text-align:center;width:72%;font-family:仿宋;font-size:14px; margin: 0 auto;">
    <tbody style="font-family:方正公文仿宋;font-size:12pt;">
    	<tr style="font-weight:normal;"> 
    		<td style="width:20%;text-align:right;">题　　目</td>
    		<td style="width:2%">：</td> 
    		<td style="width:40%;font-weight:normal;border-bottom: 1px solid;text-align:center;font-family:华文仿宋"> 概率论讲义</td>     </tr>
    	<tr style="font-weight:normal;"> 
    		<td style="width:20%;text-align:right;">姓　　名</td>
    		<td style="width:2%">：</td> 
    		<td style="width:40%;font-weight:normal;border-bottom: 1px solid;text-align:center;font-family:华文仿宋"> Elon Li</td>     </tr>
    	<tr style="font-weight:normal;"> 
    		<td style="width:20%;text-align:right;">日　　期</td>
    		<td style="width:2%">：</td> 
    		<td style="width:40%;font-weight:normal;border-bottom: 1px solid;text-align:center;font-family:华文仿宋">完成日期</td>     </tr>
    </tbody>              
    </table>
</div>

<!-- 注释语句：导出PDF时会在这里分页 -->

![概率论](C:\Users\41630\Desktop\我的笔记\我的讲义\考研数学\ProbabilityTheory\image\概率论.png)

# 目录

[TOC]

![随机事件和概率](C:\Users\41630\Desktop\我的笔记\我的讲义\考研数学\ProbabilityTheory\image\随机事件和概率.png)

## 随机事件和概率

### 事件关系

1. 包含关系$A \subset B$
2. 相等关系$A = B$
3. 和事件$A \cup B$,也记为$A+B$
4. 积事件$A\cap B$，也记为$AB$
5. 差事件$A - B$,也记为$A\overline{B}$

### 事件运算

1. 交换律$A \cup B = B \cup A,A\cap B= B \cap A$
2. 结合律$A\cup(B\cup C)= (A\cup B)\cup C;A\cap(B\cap C)= (A\cap B)\cap C$
3. 分配律$A\cup(B\cap C)= (A\cup B)\cap (A \cup C);A\cap(B\cup C)= (A\cap B)\cup (A \cap C)$
4. 德摩根律$\overline{A \cup B}=\overline{A}\cap \overline{B};\overline{A \cap B}=\overline{A}\cup \overline{B}$

### 概率的基本公式

1. $P(A-B)= P(A)-P(AB)$
2. $P(A\cup B)= P(A)+P(B)-P(AB)\\P(A\cup B\cup C)= P(A)+P(B)+P(C)-P(AB)-P(AC)-P(BC)+P(ABC)$

### 古典概型

$$
P(A) = \frac{k}{n}
$$

### 条件概型

$$
P(B \vert A) =\frac{AB}{A}
$$



### 乘法公式

$$
P(AB)=P(B \vert A)P(A)
$$

$$
P(ABC) = P(C\vert AB)P(B\vert A)P(A)
$$

### 独立性

$$
P(AB)=0 \nRightarrow A,B互相不容，A，B同时出现是不可能事件
$$



1. 已知A发生，求B发生：$P(B\vert A)$
2. A发生、B发生：$P(AB)$

### 全概率公式

$$
P(A) = \sum \limits_{i =1}^n P(B_i)P(A \vert B_i)
$$



### 贝叶斯公式

$$
P(B_j \vert A)= \frac{P(Bj)P(A\vert B_j)}{\sum\limits_{i=1}^n P(B_i)P(A\vert B_i)}
$$







![一维随机变量及其分布](C:\Users\41630\Desktop\我的笔记\我的讲义\考研数学\ProbabilityTheory\image\一维随机变量及其分布.png)

## 一维随机变量及其分布

### 离散随机分布律

| $X$   | $x_1$ | $x_2$ | $\cdots$ |
| ----- | ----- | ----- | -------- |
| $P_k$ |       |       | $\cdots$ |

### 离散随机变量分布函数

分布函数
$$
F(x) = P\{X \le x \}
$$
性质:

1. $F(x)$是一个不减函数
2. $P\{a < x \le b\} = F(b)-F(a)$
3. $0 \le F(x) \le 1$
4. $F(-\infty)=0;F(+\infty)=1$
5. $F(x)$右连续

### 常见的离散型随机变量函数分布

1. 0-1分布: $P(X = x_i)= p^{x_i}(1-p)^{1-x_i}$
2. 二项分布: $B(n,p)$: $P(X= k)=C_n^k p^k(1-o)^{n-k}$
3. 几何分布: $P(X=k)=(1-p)^{k-1}p$
4. 泊松分布: $P(X=k)=\frac{\lambda^ke^{-\lambda}}{k!}$

### 连续型随机变量

分布函数：
$$
F(x) = \int_{-\infty}^x f(t) \mathrm{d}x
$$
性质：

1. $P\{a <x \le b\} = P\{a \le x \le b\} = P\{a < x < b\} = F(b)-F(a)$
2. $P\{x > a\}= 1-F(a)$

### 连续型随机变量分布

1. 均匀分布$U(a,b)$: $f(x) = \left \{ \begin{aligned} \frac{1}{b-a},&a <x<b\\0,&其他 \end{aligned} \right.$
2. 正态分布$N(\mu,\sigma^2)$: $f(x) = \frac{1}{\sqrt{2\pi} \sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
3. 标准正态分布$N(0,1)$: $\varphi(x) = \frac{1}{\sqrt{2\pi}}e^{-\frac{(x)^2}{2}}$
4. 指数分布$e(\lambda)$: $f(x) = \left \{ \begin{aligned}\lambda e^{-\lambda x},& x > 0\\ 0,& x\le0 \end{aligned} \right.$

性质：

1. $X \sim N(\mu,\sigma^2),Z = \frac{X -\mu}{\sigma}\sim N(0,1)$
2. $P\{x_1 \le X \le x_2\} = F(x_2)-F(x_1) = \phi(\frac{x_2-\mu}{\sigma})-\phi(\frac{x_1-\mu}{\sigma})$
3. $P\{X \le x\} = P\{\frac{X-\mu}{\sigma} \le \frac{x-\mu}{\sigma}\} = \Phi(\frac{x-\mu}{\sigma})$
4. $P\{X \ge x\} = P\{\frac{X-\mu}{\sigma} \ge \frac{x-\mu}{\sigma}\} = 1-\Phi(\frac{x-\mu}{\sigma})$
5. 指数函数无记忆性：$P\{x > s+t \vert x >s\} =P\{x> t\}$

![二维随机变量及其分布](C:\Users\41630\Desktop\我的笔记\我的讲义\考研数学\ProbabilityTheory\image\二维随机变量及其分布.png)

## 二维随机变量及其分布

### 联合概率分布律

| $X \backslash Y$ | $\cdots$ | $\cdots$ | $\cdots$ | $P(X =x _i)$ |
| ---------------- | -------- | -------- | -------- | ------------ |
| $\cdots$         | $\cdots$ | $\cdots$ | $\cdots$ | $\cdots$     |
| $\cdots$         | $\cdots$ | $\cdots$ | $\cdots$ | $\cdots$     |
| $P(Y = y_i)$     | $\cdots$ | $\cdots$ | $\cdots$ | 1            |

