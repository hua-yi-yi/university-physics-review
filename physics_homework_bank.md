# 《大学物理》学习通全部作业题库与详细解析（第 2~7 章，共 27 题）

> [!NOTE]
> **课程来源**：`大学物理-软件学院2026`（教师/班级：`杨艳-2班`）  
> **数据范围**：学习通“作业”栏目下全部 **6 次作业、共 27 道简答题**（教师未公布官方答案，以下解析均已逐题重新推导与验算）。

## 作业总览表

| 章节 | 作业名称 | 题数 | 当前状态 | 成绩 | 备注 |
| :--- | :--- | :---: | :---: | :---: | :--- |
| 第二章 | 流体力学基础 | 3 题 | 已完成 | 86 分 | 全部为伯努利方程与连续性方程应用 |
| 第三章 | 液体的表面现象 | 5 题 | 已完成 | 100 分 | 表面能、附加压强、毛细现象 |
| 第四章 | 振动与波动 | 5 题 | 已完成 | 100 分 | 振动方程、旋转矢量、波动方程、波的干涉 |
| 第五章 | 静电场 | 6 题 | 已完成 | 100 分 | 场强积分、高斯定理、电势（第 3 题手写稿有一处笔误已标注） |
| 第六章 | 稳恒磁场 | 5 题 | 待批阅 | — | **发现第 3 题数值计算与第 5 题受力方向有误，下方已标红纠错** |
| 第七章 | 电磁感应定律 | 3 题 | 待做 | — | 截止时间 `2026-11-30 07:51`，下方提供完整复习推导 |

---

## 第二章 流体力学基础（共 3 题）

### 2-1（原题号 2.8）
- **原题**：一个装满水的容器的侧壁有一面积为 $1.0\times 10^{-4}\text{ m}^2$、位于水面下 $0.20\text{ m}$ 处的小孔。求从孔的出流速度及流量。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/ad0236036fa928713b80fd73bc4cb41b.png)
- **核心考点**：托里拆利公式、体积流量公式。
- **完整解析**：
  1. 由托里拆利公式（伯努利方程的特例），小孔出流速度为：
     $$v = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 0.20} = \sqrt{3.92} \approx 1.98\text{ m/s}$$
     （若取 $g = 10\text{ m/s}^2$，则 $v = 2.0\text{ m/s}$）
  2. 体积流量为：
     $$Q = Sv = 1.0\times 10^{-4} \times 1.98 \approx 1.98\times 10^{-4}\text{ m}^3/\text{s}$$

### 2-2（原题号 2-9）
- **原题**：水在截面不同的水平管中做稳定流动，出口处的截面积为管的最细处的 3 倍。若出口处的流速为 $2\text{ m}\cdot\text{s}^{-1}$，则最细处的压强为多少？若在最细处开一小孔，水会不会流出来？
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/f37934836c42d2b2e750e35104001581.png)
- **核心考点**：连续性方程 + 水平管伯努利方程。
- **完整解析**：
  1. **求最细处流速**：由连续性方程 $S_{\text{细}} v_{\text{细}} = S_{\text{出}} v_{\text{出}}$，已知 $S_{\text{出}} = 3 S_{\text{细}}$，得：
     $$v_{\text{细}} = 3 v_{\text{出}} = 3 \times 2 = 6\text{ m/s}$$
  2. **求最细处压强**：管子水平放置（$h_{\text{细}} = h_{\text{出}}$），出口通向大气（$p_{\text{出}} = p_0 = 1.013\times 10^5\text{ Pa}$）。由伯努利方程：
     $$p_{\text{细}} + \frac{1}{2}\rho v_{\text{细}}^2 = p_0 + \frac{1}{2}\rho v_{\text{出}}^2$$
     $$p_{\text{细}} = p_0 + \frac{1}{2}\times 1.0\times 10^3 \times (2^2 - 6^2) = p_0 - 1.6\times 10^4\text{ Pa} \approx 8.53\times 10^4\text{ Pa}$$
  3. **开孔判断**：因为最细处管内压强 $p_{\text{细}} < p_0$（低于外界大气压），所以开小孔后**水不会流出来**，反而外界空气会被压入（吸入）管内。

### 2-3（原题号 2-10）
- **原题**：匀速地将流量为 $Q=1.5\times 10^{-4}\text{ m}^3\cdot\text{s}^{-1}$ 的水注入一容器中，容器底有一面积为 $S=0.5\times 10^{-4}\text{ m}^2$ 的小孔，使水不断流出，试求：该容器的深度至少为多少米水才不会溢出？
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/90fb3dbd7f78ce00b0d574e303ce9f61.png)
- **核心考点**：稳态进出流量平衡 + 托里拆利公式。
- **完整解析**：
  水不溢出的临界条件是：水面达到容器深度 $h$ 时，底部流出流量刚好等于注入流量 $Q$：
  $$Q = Sv = S\sqrt{2gh}$$
  解得容器最小深度：
  $$h = \frac{Q^2}{2gS^2} = \frac{(1.5\times 10^{-4})^2}{2\times 9.8\times (0.5\times 10^{-4})^2} = \frac{9}{19.6} \approx 0.459\text{ m}$$
  （若取 $g=10\text{ m/s}^2$，则 $h = 0.45\text{ m}$。）

---

## 第三章 液体的表面现象（共 5 题）

### 3-1（原题号 3.6）
- **原题**：吹一个直径为 $10\text{ cm}$ 的肥皂泡，设肥皂液的表面张力系数 $\alpha=40\times 10^{-3}\text{ N/m}$，试求吹此肥皂泡所做的功，以及泡内外的压强差。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/3f73e988673555f4f9fa713f5005581c.png)
- **核心考点**：表面能做功、拉普拉斯公式（**肥皂泡有内外两个液面！**）。
- **完整解析**：
  已知半径 $r = d/2 = 5\text{ cm} = 0.05\text{ m}$。
  1. **吹泡做功**：肥皂泡有内外两个球面，总新增表面积 $\Delta S = 2 \times 4\pi r^2 = 8\pi r^2$：
     $$W = \alpha \Delta S = 8\pi\alpha r^2 = 8\pi \times 40\times 10^{-3} \times (0.05)^2 \approx 2.51\times 10^{-3}\text{ J}$$
  2. **泡内外压强差**：两个球面各贡献 $\frac{2\alpha}{r}$ 的附加压强：
     $$\Delta p = \frac{4\alpha}{r} = \frac{4\times 40\times 10^{-3}}{0.05} = 3.2\text{ Pa}$$

### 3-2（原题号 3-7）
- **原题**：在 $10\text{ km}^2$ 的湖面上，下了一场 $25\text{ mm}$ 的大雨，雨滴直径为 $1\text{ mm}$，设过程是等温的，求释放出来的能量，水的表面张力系数 $\alpha=7.3\times 10^{-2}\text{ N/m}$。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/fb1ce3becef6632261234f76ac495a8c.png)
- **核心考点**：液滴合并释放的表面能计算。
- **完整解析**：
  已知湖面积 $S_{\text{湖}} = 10\text{ km}^2 = 10^7\text{ m}^2$，雨深 $h = 25\text{ mm} = 0.025\text{ m}$，雨滴半径 $r = 0.5\text{ mm} = 5\times 10^{-4}\text{ m}$。
  1. 降雨总体积：$V = S_{\text{湖}} h = 10^7 \times 0.025 = 2.5\times 10^5\text{ m}^3$。
  2. 雨滴个数 $N = \frac{V}{\frac{4}{3}\pi r^3}$，全部雨滴总表面积为：
     $$S_{\text{总}} = N \cdot 4\pi r^2 = \frac{3V}{r} = \frac{3\times 2.5\times 10^5}{5\times 10^{-4}} = 1.5\times 10^9\text{ m}^2$$
  3. 雨滴落入湖中后，表面积减少量即 $S_{\text{总}}$，释放的表面能为：
     $$\Delta E = \alpha S_{\text{总}} = 7.3\times 10^{-2} \times 1.5\times 10^9 = 1.095\times 10^8\text{ J} \approx 1.10\times 10^8\text{ J}$$

### 3-3（原题号 3-9）
- **原题**：将内径为 $d=10^{-4}\text{ m}$ 的管子插入水银中，求水银面在管中下降的高度，水银完全不润湿管壁，水银的表面张力系数 $\alpha=4.9\times 10^{-1}\text{ N}\cdot\text{m}^{-1}$。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/70eb09ed2be894e3b1eee00d7a167fbf.png)
- **核心考点**：毛细现象高度公式。
- **完整解析**：
  已知半径 $r = d/2 = 0.5\times 10^{-4}\text{ m}$，完全不润湿时接触角 $\theta = 180^\circ$（$\cos\theta = -1$），水银密度 $\rho = 13.6\times 10^3\text{ kg/m}^3$：
  $$h = \frac{2\alpha\cos\theta}{\rho g r} = \frac{2\times 0.49 \times (-1)}{13.6\times 10^3 \times 9.8 \times 0.5\times 10^{-4}} \approx -0.147\text{ m}$$
  负号表示液面下降，故下降高度为 **$0.147\text{ m}$（$14.7\text{ cm}$）**。

### 3-4（原题号 3-10）
- **原题**：如图所示，在半径 $r=0.3\text{ mm}$ 的玻璃毛细管中注水一部分，在管的下端形成一弧面，其半径 $R=3.0\text{ mm}$，求管中所悬水柱的高度 $h$，水的表面张力系数 $\alpha=7.3\times 10^{-2}\text{ N/m}$。设水能完全润湿玻璃，且管内弯曲液面的曲率半径与管内半径相同。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/e0d300a33b33cc07d7f45a3f7c7e9453.png)
- **核心考点**：双弯曲液面的附加压强平衡。
- **完整解析**：
  - 上液面为凹面（向空气侧凹），液面下方 $B$ 点压强小于大气压：$p_B = p_0 - \frac{2\alpha}{r}$；
  - 下液面为凸弧面（向空气侧凸），液面上方 $A$ 点压强大于大气压：$p_A = p_0 + \frac{2\alpha}{R}$；
  - 由流体静压强关系 $p_A - p_B = \rho g h$，代入得：
    $$h = \frac{2\alpha}{\rho g}\left(\frac{1}{r} + \frac{1}{R}\right) = \frac{2\times 7.3\times 10^{-2}}{1.0\times 10^3 \times 9.8}\left(\frac{1}{3\times 10^{-4}} + \frac{1}{3\times 10^{-3}}\right) \approx 5.46\times 10^{-2}\text{ m} = 5.46\text{ cm}$$

### 3-5（原题号 3-11）
- **原题**：将 U 形管竖直放置，并灌入一部分水。设 U 形管两边管的内直径分别为 $10^{-3}\text{ m}$ 和 $3\times 10^{-3}\text{ m}$，水面的接触角为零，求两管水面的高度差。（水的表面张力系数为 $7.3\times 10^{-2}\text{ N/m}$）
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/5528110153a47d7cde24d4275c8c0a0e.png)
- **核心考点**：毛细管液面高度差计算。
- **完整解析**：
  两管半径分别为 $r_1 = 0.5\times 10^{-3}\text{ m}$、$r_2 = 1.5\times 10^{-3}\text{ m}$，$\cos\theta = 1$：
  $$\Delta h = h_1 - h_2 = \frac{2\alpha}{\rho g}\left(\frac{1}{r_1} - \frac{1}{r_2}\right) = \frac{2\times 7.3\times 10^{-2}}{1.0\times 10^3 \times 9.8}\left(\frac{1}{0.5\times 10^{-3}} - \frac{1}{1.5\times 10^{-3}}\right) \approx 1.99\times 10^{-2}\text{ m} \approx 2.0\text{ cm}$$

---

## 第四章 振动与波动（共 5 题）

### 4-1（原题号 4-22）
- **原题**：一简谐振动的振动曲线如图所示（$A=6\text{ m}$，$t=0$ 时 $y=-3\text{ m}$ 且向下运动，$a$ 为波谷 $y=-6\text{ m}$，$t=1\text{ s}$ 时为 $b$ 点 $y=+3\text{ m}$ 且向上运动，$t=2\text{ s}$ 时回到 $y=-3\text{ m}$ 向下运动）。求：(1) 振动初相和角频率；(2) 写出振动方程；(3) 求 $a, b$ 两点的相位；(4) $a$ 状态所对应的时刻；(5) 由旋转矢量法求出由状态 $a$ 到状态 $b$ 需要的时间。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/464073e4ec870a1e0a9d0f91236d13eb.png)
- **完整解析**：
  1. **周期、角频率与初相**：由图读出 $T = 2\text{ s}$，故 $\omega = \frac{2\pi}{T} = \pi\text{ rad/s}$。$t=0$ 时 $y_0 = -3 = -\frac{A}{2}$ 且 $v_0 < 0$：
     - 由 $\cos\varphi_0 = -\frac{1}{2}$ 且 $-\omega A\sin\varphi_0 < 0 \Rightarrow \sin\varphi_0 > 0$，旋转矢量位于第二象限，得 **$\varphi_0 = \frac{2\pi}{3}$**。
  2. **振动方程**：
     $$y = 6\cos\left(\pi t + \frac{2\pi}{3}\right)\text{ m}$$
  3. **$a, b$ 两点相位**：
     - $a$ 点为波谷（$y=-6$），旋转矢量逆时针转到负半轴：$\varphi_a = \pi$；
     - $b$ 点对应 $t=1\text{ s}$：$\varphi_b = \pi\times 1 + \frac{2\pi}{3} = \frac{5\pi}{3}$。
  4. **$a$ 状态对应时刻**：$\pi t_a + \frac{2\pi}{3} = \pi \Rightarrow t_a = \frac{1}{3}\text{ s}$。
  5. **由 $a$ 到 $b$ 所需时间**：旋转矢量逆时针转过角度 $\Delta\varphi = \varphi_b - \varphi_a = \frac{5\pi}{3} - \pi = \frac{2\pi}{3}$，故：
     $$\Delta t = \frac{\Delta\varphi}{\omega} = \frac{2\pi/3}{\pi} = \frac{2}{3}\text{ s}$$

### 4-2（原题号 4-24）
- **原题**：两个同方向的简谐振动方程分别为 $y_1=0.12\cos(\pi t+\pi/3)\text{ cm}$ 和 $y_2=0.15\cos(\pi t+\pi/4)\text{ cm}$，求合振动的振幅、初相，写出合振动表达式。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/5b294a558567967eee874f70d2d96eb2.png)
- **完整解析**：
  两振动同方向、同频率（$\omega = \pi$），由旋转矢量合成公式：
  1. **合振幅**：
     $$A = \sqrt{A_1^2 + A_2^2 + 2A_1 A_2\cos(\varphi_1 - \varphi_2)} = \sqrt{0.12^2 + 0.15^2 + 2\times 0.12\times 0.15\cos 15^\circ} \approx 0.268\text{ cm}$$
  2. **合初相**：
     $$\tan\varphi = \frac{A_1\sin\frac{\pi}{3} + A_2\sin\frac{\pi}{4}}{A_1\cos\frac{\pi}{3} + A_2\cos\frac{\pi}{4}} = \frac{0.1039 + 0.1061}{0.0600 + 0.1061} \approx 1.264 \Rightarrow \varphi \approx 0.902\text{ rad}\ (\approx 51.7^\circ)$$
  3. **合振动方程**：$y = 0.268\cos(\pi t + 0.902)\text{ cm}$。

### 4-3（原题号 4-26）
- **原题**：平面简谐波的振幅为 $5\text{ cm}$，频率为 $100\text{ Hz}$，波速为 $400\text{ m/s}$，沿 $x$ 轴正方向传播，以波源（设在坐标原点 $O$）处的质点在平衡位置且正向 $y$ 轴正方向运动时作为计时起点，求：(1) 波源的振动初相；(2) 波源的振动方程；(3) 该列平面简谐波的波动方程。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/47acafe58f3bf6933b97bd3b7d42ffda.png)
- **完整解析**：
  已知 $A = 5\text{ cm} = 0.05\text{ m}$，$\omega = 2\pi\nu = 200\pi\text{ rad/s}$，$\lambda = \frac{u}{\nu} = 4\text{ m}$。
  1. **波源初相**：$t=0$ 时 $y_0=0, v_0>0 \Rightarrow \cos\varphi_0=0, \sin\varphi_0<0 \Rightarrow \varphi_0 = -\frac{\pi}{2}$。
  2. **波源振动方程**：$y_0(t) = 0.05\cos\left(200\pi t - \frac{\pi}{2}\right)\text{ m}$（或 $5\cos(200\pi t - \pi/2)\text{ cm}$）。
  3. **波动方程**（沿 $+x$ 传播，把 $t$ 替换为 $t - x/u$）：
     $$y(x,t) = 0.05\cos\left[200\pi\left(t - \frac{x}{400}\right) - \frac{\pi}{2}\right] = 0.05\cos\left(200\pi t - \frac{\pi}{2}x - \frac{\pi}{2}\right)\text{ m}$$

### 4-4（原题号 4-28）
- **原题**：图为一平面余弦波在 $t=0$ 时刻的波形曲线（$A=0.04\text{ m}$，$\lambda=0.4\text{ m}$，$u=0.08\text{ m/s}$ 向右传播，$x=0$ 处 $y=0$，$x=0.1\text{ m}$ 处为波峰，$x=0.4\text{ m}$ 处为点 $P$；$a$ 在上升段 $0<x<0.1$，$b$ 在下降段 $0.1<x<0.2$）。求：(1) $O$ 点的振动方程；(2) 波函数；(3) $t=0$ 时 $a, b, P$ 点的运动方向；(4) $P$ 点的振动方程；(5) $P$ 点的振动图线；(6) $t=3T/4$ 时刻的波形曲线。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/188bc0ccd0c913a27ba0add53d6ff91a.png)
- **完整解析**：
  先算基本量：$T = \frac{\lambda}{u} = \frac{0.4}{0.08} = 5\text{ s}$，$\omega = \frac{2\pi}{T} = 0.4\pi\text{ rad/s}$。
  1. **$O$ 点振动方程**：波向右传播，用“上坡下、下坡上”口诀，$O$ 点在 $t=0$ 时位于上坡段，故向下运动（$y_O=0, v_O<0$），初相 $\varphi_O = +\frac{\pi}{2}$：
     $$y_O(t) = 0.04\cos\left(0.4\pi t + \frac{\pi}{2}\right)\text{ m}$$
  2. **波函数**：将 $t$ 换成 $t - \frac{x}{u} = t - \frac{x}{0.08}$：
     $$y(x,t) = 0.04\cos\left(0.4\pi t - 5\pi x + \frac{\pi}{2}\right)\text{ m}$$
  3. **$a, b, P$ 运动方向**（波向右传，“上坡下、下坡上”）：
     - $a$ 点（上坡段）：**向下**（$-y$ 方向）；
     - $b$ 点（下坡段）：**向上**（$+y$ 方向）；
     - $P$ 点（$x=0.4\text{ m}=\lambda$，与 $O$ 同相，上坡段）：**向下**（$-y$ 方向）。
  4. **$P$ 点振动方程**：将 $x=0.4\text{ m}$ 代入波函数：
     $$y_P(t) = 0.04\cos\left(0.4\pi t - 2\pi + \frac{\pi}{2}\right) = 0.04\cos\left(0.4\pi t + \frac{\pi}{2}\right)\text{ m}$$
  5. **$P$ 点振动图线**：横轴为 $t$（周期 $T=5\text{ s}$），纵轴为 $y$（振幅 $0.04\text{ m}$），从原点 $(0,0)$ 开始先向下画负正弦曲线（$t=1.25\text{ s}$ 到波谷 $-0.04$）。
  6. **$t=3T/4$ 时刻波形**：波向右平移 $\frac{3}{4}\lambda = 0.3\text{ m}$（或代入波函数得 $y = 0.04\cos(5\pi x)$），即从 $x=0$ 处为波峰 $+0.04\text{ m}$ 开始的标准余弦波形。

### 4-5（原题号 4-29）
- **原题**：图是干涉型消音器结构原理图。声波在 $A$ 点分成两路而后在 $B$ 点相遇因干涉相消。如果要消除频率为 $300\text{ Hz}$ 的发动机排气噪声，求弯道与直管道的长度之差至少应为多少？（设声波波速为 $340\text{ m/s}$）。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/0414a736fb1b695c3e2bbf0ad6c718a3.png)
- **完整解析**：
  两路声波在 $A$ 点同相分出，在 $B$ 点干涉相消的条件为波程差 $\Delta r = (2k+1)\frac{\lambda}{2}$（$k=0,1,2,\dots$）。取最小 $k=0$：
  $$\Delta l_{\min} = \frac{\lambda}{2} = \frac{u}{2\nu} = \frac{340}{2\times 300} = \frac{17}{30}\text{ m} \approx 0.567\text{ m}$$

---

## 第五章 静电场（共 6 题）

### 5-1（原题号 5-12）
- **原题**：正电荷均匀分布在长为 $L$ 的直棒上，电荷线密度为 $\lambda$，$P$ 点在直棒右侧延长线上、距直棒右端距离为 $L$，求 $P$ 点的电场强度。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/9f2d78dcdca996ebee371e47ea4606f4.png)
- **完整解析**：
  以 $P$ 点为原点向左建立坐标 $r$，直棒范围 $r \in [L, 2L]$，电荷元 $dq = \lambda\,dr$ 在 $P$ 点产生场强均水平向右：
  $$E = \int_L^{2L} \frac{\lambda\,dr}{4\pi\varepsilon_0 r^2} = \frac{\lambda}{4\pi\varepsilon_0}\left[-\frac{1}{r}\right]_L^{2L} = \frac{\lambda}{8\pi\varepsilon_0 L}$$
  方向：**沿直棒延长线向右**。

### 5-2（原题号 5-13）
- **原题**：半径为 $R$ 的上半圆环，左半环均匀带正电 $+\lambda$，右半环均匀带负电 $-\lambda$，求圆心 $O$ 处的电场强度 $E$。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/f725e1e2f22e3c5670037327b299096b.png)
- **完整解析**：
  利用对称性：左半环（$+\lambda$）在圆心产生场强指向右下方，右半环（$-\lambda$）在圆心产生场强指向右上方，两者**竖直分量相互抵消**，**水平分量向右叠加**。设圆心角 $\theta$ 从顶部向两侧量取（$0 \to \frac{\pi}{2}$）：
  $$E = 2 \int_0^{\pi/2} \frac{\lambda R\,d\theta}{4\pi\varepsilon_0 R^2}\sin\theta = \frac{\lambda}{2\pi\varepsilon_0 R}\Big[-\cos\theta\Big]_0^{\pi/2} = \frac{\lambda}{2\pi\varepsilon_0 R}$$
  方向：**水平向右**（由正电半环指向负电半环）。

### 5-3（原题号 5-14）
- **原题**：真空中有一沿 $x$ 方向的静电场 $\mathbf{E}=bx\mathbf{i}$（$b$ 为正常量），一边长为 $a$ 的立方体封闭面（左面在 $x=0$，右面 $S_1$ 在 $x=a$），求通过右侧 $S_1$ 面的电通量 $\Phi_1$、通过上表面 $S_2$ 的电通量 $\Phi_2$ 和立方体内的净电量 $Q$。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/025c25d9ce85752978c08f0af769ac95.png)
- **完整解析**：
  1. 右侧面 $S_1$ 位于 $x=a$，场强 $E = ba$ 与外法向同向：$\Phi_1 = E \cdot S_1 = ba \cdot a^2 = ba^3$；
  2. 上表面 $S_2$ 外法向沿 $+y$，与 $\mathbf{E}$ 垂直：$\Phi_2 = 0$；
  3. 左侧面在 $x=0$ 处 $E=0$，其余三面法向均垂直 $\mathbf{E}$，故总电通量 $\Phi = \Phi_1 = ba^3$。由高斯定理：
     $$Q = \varepsilon_0 \Phi = \varepsilon_0 ba^3$$
  > [!WARNING]
  > **已交作业小笔误提醒**：你之前提交的手写稿最后一行把 $Q$ 笔误写成了 $\varepsilon_0 ba^2$，正确结果应为 **$\varepsilon_0 ba^3$**，期末考试注意别丢指数！

### 5-4（原题号 5-15）
- **原题**：两个均匀带电同心球面半径分别为 $R_1=0.10\text{ m}$、$R_2=0.30\text{ m}$，带电量 $q_1=1.0\times 10^{-8}\text{ C}$、$q_2=1.5\times 10^{-8}\text{ C}$。求距球心 $r_1=0.05\text{ m}$、$r_2=0.20\text{ m}$、$r_3=0.50\text{ m}$ 处的电场强度。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/9d714629f3d853c782ad47ad5cfe5989.png)
- **完整解析**：
  由球对称性高斯定理 $E = \frac{q_{\text{内}}}{4\pi\varepsilon_0 r^2} = k\frac{q_{\text{内}}}{r^2}$（$k=9\times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$）：
  - $r_1 = 0.05\text{ m} < R_1$：$q_{\text{内}} = 0 \Rightarrow E_1 = 0$；
  - $R_1 < r_2 = 0.20\text{ m} < R_2$：$q_{\text{内}} = q_1 \Rightarrow E_2 = \frac{9\times 10^9 \times 1.0\times 10^{-8}}{0.20^2} = 2.25\times 10^3\text{ N/C}$（径向向外）；
  - $r_3 = 0.50\text{ m} > R_2$：$q_{\text{内}} = q_1 + q_2 = 2.5\times 10^{-8}\text{ C} \Rightarrow E_3 = \frac{9\times 10^9 \times 2.5\times 10^{-8}}{0.50^2} = 9.0\times 10^2\text{ N/C}$（径向向外）。

### 5-5（原题号 5-17）
- **原题**：真空中两块互相平行的无限大均匀带电平板，电荷面密度分别为 $+\sigma$ 和 $+2\sigma$，求板间电场强度大小。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/3487980595fec2e52785e02572e96092.png)
- **完整解析**：
  单块无限大带电平板场强大小为 $E = \frac{\sigma}{2\varepsilon_0}$（正电荷向外）。两板均带正电，在板间区域两者场强方向相反，叠加得：
  $$E = \frac{2\sigma}{2\varepsilon_0} - \frac{\sigma}{2\varepsilon_0} = \frac{\sigma}{2\varepsilon_0}$$
  （方向由 $+2\sigma$ 板指向 $+\sigma$ 板）。

### 5-6（原题号 5-18）
- **原题**：半径为 $R$ 的均匀带电圆环，电荷线密度为 $\lambda$，设无穷远处为电势零点，求圆环中心点的电势。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/19b6e66bff2ee9f935742e1e84f3ad30.png)
- **完整解析**：
  圆环上每个电荷元 $dq$ 到圆心距离均为 $R$，电势为标量直接相加：
  $$U = \oint \frac{dq}{4\pi\varepsilon_0 R} = \frac{Q}{4\pi\varepsilon_0 R} = \frac{\lambda \cdot 2\pi R}{4\pi\varepsilon_0 R} = \frac{\lambda}{2\varepsilon_0}$$

---

## 第六章 稳恒磁场（共 5 题）

### 6-1（原题号 6-14）
- **原题**：载有电流 $I$ 的无限长直导线一侧有一共面等腰直角三角形回路 $MNO$，$MN$ 边与导线平行且相距为 $a$，$MN = MO = a$，求通过此回路的磁通量。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/630c625f8be28e2a9c7b0737579c4602.png)
- **完整解析**：
  距直导线 $x$ 处磁感应强度 $B = \frac{\mu_0 I}{2\pi x}$（垂直纸面向里）。在 $x \in [a, 2a]$ 处取宽 $dx$ 的竖直窄条，高度 $h(x) = 2a - x$：
  $$\Phi = \int_a^{2a} \frac{\mu_0 I}{2\pi x}(2a - x)\,dx = \frac{\mu_0 I}{2\pi}\Big[2a\ln x - x\Big]_a^{2a} = \frac{\mu_0 Ia}{2\pi}(2\ln 2 - 1)$$
  方向：**垂直纸面向里**。

### 6-2（原题号 6-16）
- **原题**：无限长直导线弯成如图所示形状（半无限长直导线 $ab$ + 半径 $R$ 的四分之一圆弧 $bc$ + 延长线过圆心 $O$ 的半无限长直导线 $cd$），$I=10\text{ A}$，$R=5\text{ cm}$，求环心 $O$ 点的磁感应强度。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/c602b5739eae7461b089f8d21a39c2ff.png)
- **完整解析**：
  分段叠加（垂直纸面向里为正）：
  1. 半无限长直导线 $ab$：$B_1 = \frac{\mu_0 I}{4\pi R}$（向里）；
  2. 四分之一圆弧 $bc$：$B_2 = \frac{1}{4}\cdot\frac{\mu_0 I}{2R} = \frac{\mu_0 I}{8R}$（向里）；
  3. 直导线 $cd$ 延长线过 $O$ 点：$B_3 = 0$。
  $$B = B_1 + B_2 = \frac{\mu_0 I}{4\pi R}\left(1 + \frac{\pi}{2}\right) = \frac{4\pi\times 10^{-7}\times 10}{4\pi\times 0.05}\left(1 + \frac{\pi}{2}\right) \approx 5.14\times 10^{-5}\text{ T}$$
  方向：**垂直纸面向里**。

### 6-3（原题号 6-19）
- **原题**：真空中 $10\text{ A}$ 的电流沿轴线方向流过极长的圆柱形导体，横截面（直径 $d=4\text{ cm}$）上电流均匀分布，求磁场中磁感应强度最大的位置及最大值。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/d8508e410c08e2ee53023b0fed567aa6.png)
- **完整解析**：
  由安培环路定理：柱内（$r \le R$）$B = \frac{\mu_0 I r}{2\pi R^2}$（随 $r$ 线性增大）；柱外（$r \ge R$）$B = \frac{\mu_0 I}{2\pi r}$（随 $r$ 反比减小）。
  - **最大位置**：圆柱导体表面 $r = R = \frac{d}{2} = 2\text{ cm} = 0.02\text{ m}$ 处。
  - **最大值**：
    $$B_{\max} = \frac{\mu_0 I}{2\pi R} = \frac{4\pi\times 10^{-7} \times 10}{2\pi \times 0.02} = 1.0\times 10^{-4}\text{ T}$$
  > [!CAUTION]
  > **已交作业纠错**：你提交的答案中把 $B_{\max}$ 算成了 $5\times 10^{-5}\text{ T}$（误把直径 $0.04\text{ m}$ 当半径代了，或少乘了 2）。记住 $\frac{\mu_0}{2\pi} = 2\times 10^{-7}$，代入 $R=0.02\text{ m}$ 正确结果是 **$1.0\times 10^{-4}\text{ T}$**！

### 6-4（原题号 6-20）
- **原题**：载流体横截面中，电流方向垂直纸面向外，加铅直向上磁场 $\vec{B}$，结果左侧堆积负电荷、右侧堆积正电荷，问载流体中运动电荷的性质。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/58ffd7bc2e35fec3af7433af36fea3c3.png)
- **完整解析**：
  **霍尔效应判断法**：不管载流子带正电还是负电，只要电流方向确定，洛伦兹力 $\vec{F} = q\vec{v}\times\vec{B}$ 的偏转方向总是一致的！
  - 电流垂直纸面向外、$\vec{B}$ 向上：用左手定则（或假设正电荷向外运动，$\vec{v}\times\vec{B}$ 向左），可知**所有运动载流子都会向左偏转**；
  - 既然左侧堆积的是负电荷，说明向左偏转的载流子带**负电（自由电子）**。

### 6-5（原题号 6-21）
- **原题**：载有电流 $I_1$（向上）的长直导线旁有一共面等腰三角形回路（顺时针电流 $I_2$），顶点 $C$ 距导线 $a$，底边 $DE$ 长 $d$、平行于导线且相距 $b$，求回路所受磁力。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/64eae3a52ba60be0450aa9d8ba56f0cc.png)
- **完整解析**：
  1. 底边 $DE$ 电流向下（与 $I_1$ 反向），受**向右斥力**：
     $$F_{DE} = \frac{\mu_0 I_1 I_2 d}{2\pi b}$$
  2. 两斜边 $CD$、$EC$ 的竖直方向受力对称抵消；两斜边电流均有竖直向上分量（与 $I_1$ 同向），故均受**向左引力**。在距离 $x \in [a, b]$ 处，两斜边竖直投影总微元 $dy_{\text{总}} = \frac{d}{b-a}\,dx$：
     $$F_{\text{斜}} = \int_a^b \frac{\mu_0 I_1 I_2}{2\pi x}\cdot\frac{d}{b-a}\,dx = \frac{\mu_0 I_1 I_2 d}{2\pi(b-a)}\ln\frac{b}{a}$$
  3. 因为斜边整体离导线更近（$\frac{\ln(b/a)}{b-a} > \frac{1}{b}$），所以**向左引力大于向右斥力**，合力为：
     $$F = F_{\text{斜}} - F_{DE} = \frac{\mu_0 I_1 I_2 d}{2\pi}\left(\frac{\ln(b/a)}{b-a} - \frac{1}{b}\right)$$
     方向：**垂直于长直导线向左（指向长直导线，即吸引力）**。
  > [!CAUTION]
  > **已交作业纠错**：你提交的答案大小公式完全正确，但方向误写成了“远离直导线（斥力）”。记住：**离直导线越近磁场越强**，斜边与 $I_1$ 同向相吸且离得更近，所以合力一定是**吸引力（指向直导线）**！

---

## 第七章 电磁感应定律（共 3 题｜当前待做，截止 11-30）

### 7-1（原题号 7-17）
- **原题**：长直载流导线 $PQ$ 旁有一共面矩形导体框 $ABCD$，边长 $AB=a$、$BC=b$，$AD$ 边距 $PQ$ 为 $l$。$PQ$ 中电流 $I=I_0+kt$（$I_0, k$ 为正常量，方向向上）。求任意时刻 $t$ 线框 $ABCD$ 上的感应电动势。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/c9b43c5e56f981d1d417e2436952f124.png)
- **完整解析**：
  1. **求任意时刻磁通量**（取垂直纸面向里为正）：
     $$\Phi(t) = \int_l^{l+a} \frac{\mu_0 I}{2\pi x}\cdot b\,dx = \frac{\mu_0 b (I_0 + kt)}{2\pi}\ln\frac{l+a}{l}$$
  2. **求感应电动势**（法拉第电磁感应定律）：
     $$\mathcal{E} = -\frac{d\Phi}{dt} = -\frac{\mu_0 k b}{2\pi}\ln\frac{l+a}{l}$$
  - **大小**：$\mathcal{E} = \frac{\mu_0 k b}{2\pi}\ln\left(1 + \frac{a}{l}\right)$（与 $t$ 无关，为恒定值）。
  - **方向**：因 $k>0$，向里磁通量增大，由楞次定律，感应电动势方向为**逆时针**（$A\to D\to C\to B\to A$）。

### 7-2（原题号 7-18）
- **原题**：水平金属棒 $ab=0.5\text{ m}$，绕通过棒上 $M$ 点的竖直轴 $OO'$ 在水平面内以 $\omega=4\pi\text{ rad/s}$ 匀角速度转动，$aM=0.1\text{ m}$。竖直向上磁场 $B=0.5\times 10^{-4}\text{ T}$，求 $ab$ 两端的电势差。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/fe77bd89a7c4c76a96eaf029a4b1e82c.png)
- **完整解析**：
  1. 绕端点旋转的直棒动生电动势公式：$\mathcal{E} = \frac{1}{2}B\omega L^2$。
  2. 将棒以转轴 $M$ 分成 $Ma$（长 $l_1 = 0.1\text{ m}$）和 $Mb$（长 $l_2 = 0.5 - 0.1 = 0.4\text{ m}$）两段。由于两段同向绕 $M$ 旋转，两段感应电动势方向均从轴心指向端点（或均从端点指向轴心），在整根棒上**方向相反、互相抵消**：
     $$|U_{ab}| = |\mathcal{E}_{Mb} - \mathcal{E}_{Ma}| = \frac{1}{2}B\omega\left(l_2^2 - l_1^2\right)$$
  3. 代入数值：
     $$|U_{ab}| = \frac{1}{2} \times 0.5\times 10^{-4} \times 4\pi \times (0.4^2 - 0.1^2) = \pi\times 10^{-4} \times 0.15 = 1.5\pi\times 10^{-5}\text{ V} \approx 4.71\times 10^{-5}\text{ V}$$
  - **高低电势判断**：若俯视逆时针转动，$\vec{v}\times\vec{B}$ 从轴心 $M$ 指向两端，$b$ 端电势高于 $a$ 端；若俯视顺时针转动，$\vec{v}\times\vec{B}$ 从两端指向轴心 $M$，$a$ 端电势高于 $b$ 端（写作业时对照原图 $\omega$ 箭头方向即可确定）。

### 7-3（原题号 7-19）
- **原题**：无限长直导线通以向上稳恒电流 $I$，右侧倾斜直棒 $ab$ 长 $L$，最近端 $a$ 距直导线 $d$，$ab$ 与水平线夹角为 $\alpha$。使 $ab$ 沿与长直导线平行的方向以速度 $\vec{v}$ 向上运动，求其中的感应电动势。
- **原题图片**：[查看原图](https://p.ananas.chaoxing.com/star3/origin/b4ada6650b8149ef85d57653170e27f1.png)
- **完整解析**：
  1. 在棒上距 $a$ 端 $l$ 处取微元 $dl$，它到长直导线的水平距离为 $r = d + l\cos\alpha$，该处磁场 $B = \frac{\mu_0 I}{2\pi r}$（垂直纸面向里）。
  2. $\vec{v}$ 竖直向上，$\vec{B}$ 向里，故非静电力方向 $\vec{v}\times\vec{B}$ **水平向左**，大小为 $vB$。微元 $d\vec{l}$ 沿棒方向与 $\vec{v}\times\vec{B}$ 夹角为 $\alpha$（取从 $b\to a$ 为正方向，夹角为 $\alpha$），有效切割长度即水平投影 $dr = dl\cos\alpha$：
     $$\mathcal{E} = \int_0^L vB\cos\alpha\,dl = \int_d^{d+L\cos\alpha} \frac{\mu_0 I v}{2\pi r}\,dr = \frac{\mu_0 I v}{2\pi}\ln\frac{d + L\cos\alpha}{d}$$
  3. **方向**：由 $b$ 指向 $a$，即 **$a$ 端电势高于 $b$ 端**。
