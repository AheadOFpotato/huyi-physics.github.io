---
title: class1
category: optic discussion
order: 2
---
<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
</script>
</head>
<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

[toc]

# motivation
量子霍尔效应 QHE: 分数QHE(fQHE) + 整数iQHE
--> QH insulator (property: bulk insulating; edge conduct)
-->最关键的：要使得电子在里面回转运动 vortex motion(看似是需要磁场，其实是因为下面的根本原因，看起来需要很强很强的磁场1-10T，不太可能，therefore👇)
--> 这个运动根本生对应着 TRSB 时间反演对称性破缺
--> 因而只需要保留TRSB Haldame：不需要磁场的量子霍尔效应

logic : QHE --> QH insulator --光学模拟--> 拓扑光子学
# outline
* QHE experiment 经典霍尔效应和量子霍尔效应如何过渡 ?
* (朗道能级引入-->) edge mode(霍尔电导量子化的性质), basic interpretation
  * 拓扑
    * manifold ; fiber bundle 定义在某些几何图形上的矢量函数(某种多值矢量函数)
    * connection ; curvature 纤维的曲率沿着几何图形(e.g.环面)积分积出来是一个整数 --由下面的东西导出-->
    * 上同调 ———— TKNN

# lecture 1
## 经典霍尔效应
电子器：一堆自由电子 x - -y 平面
磁场 + 垂直的电场 --> 产生的电流叫霍尔电流
$$\sigma_H = \sigma_xy = -\frac{\sigma_0}{\omega_C\tau}=-\frac{ne^2\tau}{m^*}\frac{m^*}{eB}\frac{1}{\tau}=-\frac{ne}{B}$$

$$\sigma_H(n,B)$$
* 整数量子效应（完整平台）
* 分数量子效应（断断续续平台）
* 平台是因为没有体态电流 Ix(电场方向电流)
<font color=yellow>为什么体态是x方向</font>
在边缘和体态都有电流