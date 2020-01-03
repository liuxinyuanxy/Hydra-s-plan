# $\color{red}\text{Hydra's plan}$

about me:

​	这是$\text{Hydra}$的学习/复习计划，主要为知识点与她做过的题，某些题后面可能跟着她的做法

## $\color{blue}\text{The first month}$

### $省选进阶数据结构与动态树$

###### 树套树

###### 可持久化数据结构

###### 根号平衡

序列$O(1)$单点修改，$O(\sqrt n)$区间和

序列$O(\sqrt n)$单点修改，$O(1)$区间和

序列$O(\sqrt n)$区间加，$O(1)$求单点

序列$O(1)$区间加，$O(\sqrt n)$求单点

集合$O(1)$插入，$O(\sqrt n)$查第$k$小

集合$O(\sqrt n)$插入，$O(1)$查第$k$小



最后一个问题很有意思，写一下我的做法

维护一个排好序的双向链表

分$\sqrt n$块，第$i$块维护的左右端点为$l_i,r_i(r_i-l_i=\sqrt n)$，记录排名为$l_i$和$r_i$的位置$p_l,p_r$

插入时$O(\sqrt n)$找到插入的位置，然后$O(\sqrt n)$修改后面的块的$p_l$和$p_r$(集体前移一位)

注意边界即可

###### 普通、树上、带修、不删除、二维、二次离线莫队

[洛谷P3245](https://www.luogu.com.cn/problem/P3245)

[洛谷P4396](https://www.luogu.com.cn/problem/P4396)

[CF617E](http://codeforces.com/contest/617/problem/E)

[洛谷P4074](https://www.luogu.com.cn/problem/P4074)

###### 复杂的分块问题(特指$\text{Ynoi}$)

###### 点分治、链分治、$\text{LCT}$、静态$\text{LCT}$、静态$\text{top tree}$

[洛谷P2634](https://www.luogu.com.cn/problem/P2634)

[洛谷P2056](https://www.luogu.com.cn/problem/P2056),[洛谷P4115](https://www.luogu.com.cn/problem/P4115),[洛谷SP2666](https://www.luogu.com.cn/problem/SP2666)(喜闻乐见的三倍经验qwq)

[bzoj3730](https://lydsy.com/JudgeOnline/problem.php?id=3730)

这道傻逼题卡了我好几天(其实主要原因是参加合格考qwq)，写一下吧

要求距离节点$x$不超过$k$的权值和

很容易想到动态点分治，在分治中心使用两个数据结构分别维护距离分治中心和分治中心的父亲距离不超过$i$的节点的权值和

一开始我想用动态开点线段树做，但这样做空间复杂度是$O(n\log ^2n)$的，好像不太行

于是我用$\text{Splay}$维护，空间复杂度$O(n\log n)$，时间$O(n\log ^2 n)$。但是可能是因为代码写丑了，死活过不去

但是！在我回教室的路上，我突然想到，每个线段树的值域只需要开到**距分治中心最远点的深度**就可以了，空间其实可以做到$O(n\log n)$。而且，这样甚至只需要用树状数组维护就可以了。

[bzoj4372](https://lydsy.com/JudgeOnline/problem.php?id=4372)

[洛谷P1501](https://www.luogu.com.cn/problem/P1501)

[洛谷P3203](https://www.luogu.com.cn/problem/P3203)

[洛谷P3950](https://www.luogu.com.cn/problem/P3950),[洛谷P2147](https://www.luogu.com.cn/problem/P2147)

## $\color{blue}\text{The second month}$

### $数学相关$

###### 线性代数

###### 线性规划

###### 莫比乌斯反演与杜教筛

###### 多项式相关($\text{FFT}$、字符串匹配问题、分治$\text{FFT}$、多项式求逆等)

### $图论相关$

###### 网络流

###### 树上问题(这个可能应该放到数据结构里？)

## $\color{blue}\text{The third month}$

### $高阶动态规划$

###### 状压、轮廓线、数位DP

###### 倍增、数据结构、单调队列、决策单调性、斜率优化DP

### $字符串$

###### 回文自动机

###### AC自动机

###### 后缀数组

###### 后缀自动机

## $\color{blue}\text{The fourth month}$

### $\displaystyle 刷套题，查缺补漏$

