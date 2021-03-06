---
layout: article
title:  LaTex formula
date:   2017-04-11
categories: articles
image:
 teaser: latex.jpg
---
>##### 摘要：LaTex公式汇总速查

---
[1.强调模式](#1)
[2.希腊字母](#2)
[3.二元运算](#3)
[4.关系运算](#4)
[5.箭头符号](#5)
[6.杂类符号](#6)
[7.特殊符号](#7)
[8.曲线函数](#8)
[9.分隔符号](#9)
[10.数学结构](#10)
[11.AMS希腊字母](#11)
[12.AMS分隔符号](#12)
[13.AMS箭头符号](#13)
[14.AMS二元关系符](#14)
[15.AMS二元操作符](#15)
[16.AMS杂类符号](#16)

由于在写电子笔记的时候经常要写入公式，MS全家桶的公式编辑器虽然容易上手够用，但是在较复杂的公式上书写不自如，尽管LaTex公式比较复杂，但是付出了刚上手的学习成本之后就能行云流水了，加上Markdown支持LaTex公式，而且它语法不像LaTex复杂，也不需要编译，俩合一起简直就是行云流水小进攻。下面就是一些LaTex公式的书写，这么多很常用的肯定是要记的，其它的到时候查吧，但也不需要刻意记，无他，唯手熟尔。

##### <h2 id="1">强调模式</h2>
>$\hat{a}&ensp;\text{\hat{a}}&ensp;&ensp;
\acute{a}&ensp;\text{\acute{a}}&ensp;&ensp;
\bar{a}&ensp;\text{\bar{a}}&ensp;&ensp;
\dot{a}&ensp;\text{\dot{a}}&ensp;&ensp;
\breve{a}&ensp;\text{\breve{a}}&ensp;&ensp;\\
\check{a}&ensp;\text{\check{a}}&ensp;&ensp;
\grave{a}&ensp;\text{\grave{a}}&ensp;&ensp;
\vec{a}&ensp;\text{\vec{a}}&ensp;&ensp;
\ddot{a}&ensp;\text{\ddot{a}}&ensp;&ensp;
\tilde{a}&ensp;\text{\tilde{a}}$

##### <h2 id="2">希腊字母</h2>
>$\alpha&ensp;\text{\alpha}&ensp;&ensp;
\beta&ensp;\text{\beta}&ensp;&ensp;
\gamma&ensp;\text{\gamma}&ensp;&ensp;
\delta&ensp;\text{\delta}&ensp;&ensp;
\epsilon&ensp;\text{\epsilon}&ensp;&ensp;\\
\varepsilon&ensp;\text{\varepsilon}&ensp;&ensp;
\zeta&ensp;\text{\zeta}&ensp;&ensp;
\eta&ensp;\text{\eta}&ensp;&ensp;
\theta&ensp;\text{\theta}&ensp;&ensp;
\vartheta&ensp;\text{\vartheta}&ensp;&ensp;\\
\iota&ensp;\text{\iota}&ensp;&ensp;
\kappa&ensp;\text{\kappa}&ensp;&ensp;
\lambda&ensp;\text{\lambda}&ensp;&ensp;
\mu&ensp;\text{\mu}&ensp;&ensp;
\nu&ensp;\text{\nu}&ensp;&ensp;\\
\xi &ensp;\text{\xi}&ensp;&ensp;&ensp;
o&ensp;\text{o}&ensp;&ensp;
\pi&ensp;\text{\pi}&ensp;&ensp;
\varpi&ensp;\text{\varpi}&ensp;&ensp;
\rho&ensp;\text{\rho}&ensp;&ensp;\\
\varrho  &ensp;\text{\varrho}&ensp;&ensp;
\sigma&ensp;\text{\sigma}&ensp;&ensp;
\varsigma&ensp;\text{\varsigma}&ensp;&ensp;
\tau&ensp;\text{\tau}&ensp;&ensp;
\upsilon&ensp;\text{\upsilon}&ensp;&ensp;\\
\phi  &ensp;\text{\phi}&ensp;&ensp;
\varphi&ensp;\text{\varphi}&ensp;&ensp;
\chi&ensp;\text{\chi}&ensp;&ensp;
\psi&ensp;\text{\psi}&ensp;&ensp;
\omega&ensp;\text{\omega}&ensp;&ensp;\\
\Gamma &ensp;\text{\Gamma}&ensp;&ensp;
\Delta&ensp;\text{\Delta}&ensp;&ensp;
\Theta&ensp;\text{\Theta}&ensp;&ensp;
\Lambda&ensp;\text{\Lambda}&ensp;&ensp;
\Xi&ensp;\text{\Xi}&ensp;&ensp;\\
\Pi&ensp;\text{\Pi}&ensp;&ensp;
\Sigma&ensp;\text{\Sigma}&ensp;&ensp;
\Upsilon&ensp;\text{\Upsilon}&ensp;&ensp;
\Phi&ensp;\text{\Phi}&ensp;&ensp;
\Psi&ensp;\text{\Psi}&ensp;&ensp;\\
\Omega&ensp;\text{\Omega}&ensp;&ensp;$

##### <h2 id="3">二元运算</h2>
>$\pm&ensp;\text{\pm}&ensp;&ensp;
\cap&ensp;\text{\cap}&ensp;&ensp;
\diamond&ensp;\text{\diamond}&ensp;&ensp;
\oplus&ensp;\text{\oplus}&ensp;&ensp;
\mp&ensp;\text{\mp}&ensp;&ensp;\\
\cup&ensp;\text{\cup}&ensp;&ensp;
\bigtriangleup&ensp;\text{\bigtriangleup}&ensp;&ensp;
\ominus&ensp;\text{\ominus}&ensp;&ensp;
\times  &ensp;\text{\times}&ensp;&ensp;
\uplus&ensp;\text{\uplus}&ensp;&ensp;\\
\bigtriangledown&ensp;\text{\bigtriangledown}&ensp;&ensp;
\otimes&ensp;\text{\otimes}&ensp;&ensp;
\div &ensp;\text{\div}&ensp;&ensp;
\sqcap&ensp;\text{\sqcap}&ensp;&ensp;
\triangleleft&ensp;\text{\triangleleft}&ensp;&ensp;\\
\oslash&ensp;\text{\oslash}&ensp;&ensp;
\ast  &ensp;\text{\ast}&ensp;&ensp;
\sqcup&ensp;\text{\sqcup}&ensp;&ensp;
\triangleright&ensp;\text{\triangleright}&ensp;&ensp;
\odot&ensp;\text{\odot}&ensp;&ensp;\\
\star  &ensp;\text{\star}&ensp;&ensp;
\vee&ensp;\text{\vee}&ensp;&ensp;
\lhd&ensp;\text{\lhd}^{a}&ensp;&ensp;
\bigcirc&ensp;\text{\bigcirc}&ensp;&ensp;
\circ  &ensp;\text{\circ}&ensp;&ensp;\\
\wedge&ensp;\text{\wedge}&ensp;&ensp;
\rhd&ensp;\text{\rhd}^{a}&ensp;&ensp;
\dagger&ensp;\text{\dagger}&ensp;&ensp;
\bullet  &ensp;\text{\bullet}&ensp;&ensp;
\setminus&ensp;\text{\setminus}&ensp;&ensp;\\
\unlhd&ensp;\text{\unlhd}^{a}&ensp;&ensp;
\ddagger&ensp;\text{\ddagger}&ensp;&ensp;
\cdot  &ensp;\text{\cdot}&ensp;&ensp;
\wr&ensp;\text{\wr}&ensp;&ensp;
\unrhd&ensp;\text{\unrhd}^{a}&ensp;&ensp;$

##### <h2 id="4">关系运算</h2>
>$\leq&ensp;\text{\leq,\le}&ensp;&ensp;
\geq&ensp;\text{\geq,\ge}&ensp;&ensp;
\equiv&ensp;\text{\equiv}&ensp;&ensp;
\models&ensp;\text{\models}&ensp;&ensp;
\prec&ensp;\text{\prec}&ensp;&ensp;\\
\succ&ensp;\text{\succ}&ensp;&ensp;
\sim&ensp;\text{\sim}&ensp;&ensp;
\perp&ensp;\text{\perp}&ensp;&ensp;
\preceq&ensp;\text{\preceq}&ensp;&ensp;
\succeq&ensp;\text{\succeq}&ensp;&ensp;\\
\simeq&ensp;\text{\simeq}&ensp;&ensp;
\mid&ensp;\text{\mid}&ensp;&ensp;
\ll&ensp;\text{\ll}&ensp;&ensp;
\gg&ensp;\text{\gg}&ensp;&ensp;
\asymp&ensp;\text{\asymp}&ensp;&ensp;\\
\parallel&ensp;\text{\parallel}&ensp;&ensp;
\subset&ensp;\text{\subset}&ensp;&ensp;
\supset&ensp;\text{\supset}&ensp;&ensp;
\approx&ensp;\text{\approx}&ensp;&ensp;
\bowtie&ensp;\text{\bowtie}&ensp;&ensp;\\
\subseteq&ensp;\text{\subseteq}&ensp;&ensp;
\supseteq&ensp;\text{\supseteq}&ensp;&ensp;
\cong&ensp;\text{\cong}&ensp;&ensp;
\Join&ensp;\text{\Join}&ensp;&ensp;
\sqsubset&ensp;\text{\sqsubset}&ensp;&ensp;\\
\sqsupset&ensp;\text{\sqsupset}&ensp;&ensp;
\neq&ensp;\text{\neq}&ensp;&ensp;
\smile&ensp;\text{\smile}&ensp;&ensp;
\sqsubseteq&ensp;\text{\sqsubseteq}&ensp;&ensp;
\sqsupseteq&ensp;\text{\sqsupseteq}&ensp;&ensp;\\
\doteq&ensp;\text{\doteq}&ensp;&ensp;
\frown&ensp;\text{\frown}&ensp;&ensp;
\in&ensp;\text{\in}&ensp;&ensp;
\ni&ensp;\text{\ni}&ensp;&ensp;
\propto&ensp;\text{\propto}&ensp;&ensp;\\
=&ensp;\text{=}&ensp;&ensp;
\vdash&ensp;\text{\vdash}&ensp;&ensp;
\dashv&ensp;\text{\dashv}&ensp;&ensp;
<&ensp;\text{<}&ensp;&ensp;
>&ensp;\text{>}&ensp;&ensp;$

##### <h2 id="5">箭头符号</h2>
>$\leftarrow&ensp;\text{\leftarrow}&ensp;&ensp;
\longleftarrow&ensp;\text{\longleftarrow}&ensp;&ensp;
\uparrow&ensp;\text{\uparrow}&ensp;&ensp;
\Leftarrow&ensp;\text{\Leftarrow}&ensp;&ensp;
\Longleftarrow&ensp;\text{\Longleftarrow}&ensp;&ensp;\\
\Uparrow&ensp;\text{\Uparrow}&ensp;&ensp;
\rightarrow&ensp;\text{\rightarrow}&ensp;&ensp;
\longrightarrow&ensp;\text{\longrightarrow}&ensp;&ensp;
\downarrow&ensp;\text{\downarrow}&ensp;&ensp;
\Rightarrow&ensp;\text{\Rightarrow}&ensp;&ensp;\\
\Longrightarrow&ensp;\text{\Longrightarrow}&ensp;&ensp;
\Downarrow&ensp;\text{\Downarrow}&ensp;&ensp;
\leftrightarrow&ensp;\text{\leftrightarrow}&ensp;&ensp;
\longleftrightarrow&ensp;\text{\longleftrightarrow}&ensp;&ensp;
\updownarrow&ensp;\text{\updownarrow}&ensp;&ensp;\\
\Leftrightarrow&ensp;\text{\Leftrightarrow}&ensp;&ensp;
\Longleftrightarrow&ensp;\text{\Longleftrightarrow}&ensp;&ensp;
\Updownarrow&ensp;\text{\Updownarrow}&ensp;&ensp;
\mapsto&ensp;\text{\mapsto}&ensp;&ensp;
\longmapsto&ensp;\text{\longmapsto}&ensp;&ensp;\\
\nearrow&ensp;\text{\nearrow}&ensp;&ensp;
\hookleftarrow&ensp;\text{\hookleftarrow}&ensp;&ensp;
\hookrightarrow&ensp;\text{\hookrightarrow}&ensp;&ensp;
\searrow&ensp;\text{\searrow}&ensp;&ensp;
\leftharpoonup&ensp;\text{\leftharpoonup}&ensp;&ensp;\\
\rightharpoonup&ensp;\text{\rightharpoonup}&ensp;&ensp;
\swarrow&ensp;\text{\swarrow}&ensp;&ensp;
\leftharpoondown&ensp;\text{\leftharpoondown}&ensp;&ensp;
\rightharpoondown&ensp;\text{\rightharpoondown}&ensp;&ensp;
\nwarrow&ensp;\text{\nwarrow}&ensp;&ensp;\\$

##### <h2 id="6">杂类符号</h2>
>$\ldots&ensp;\text{\ldots}&ensp;&ensp;
\cdots&ensp;\text{\cdots}&ensp;&ensp;
\vdots&ensp;\text{\vdots}&ensp;&ensp;
\ddots&ensp;\text{\ddots}&ensp;&ensp;
\aleph&ensp;\text{\aleph}&ensp;&ensp;\\
\prime&ensp;\text{\prime}&ensp;&ensp;
\forall&ensp;\text{\forall}&ensp;&ensp;
\infty&ensp;\text{\infty}&ensp;&ensp;
\hbar&ensp;\text{\hbar}&ensp;&ensp;
\emptyset&ensp;\text{\emptyset}&ensp;&ensp;\\
\exists&ensp;\text{\exists}&ensp;&ensp;
\nabla&ensp;\text{\nabla}&ensp;&ensp;
\surd&ensp;\text{\surd}&ensp;&ensp;
\Box&ensp;\text{\Box}^{a}&ensp;&ensp;
\triangle&ensp;\text{\triangle}&ensp;&ensp;\\
\Diamond&ensp;\text{\Diamond}^{a}&ensp;&ensp;
\imath&ensp;\text{\imath}&ensp;&ensp;
\jmath&ensp;\text{\jmath}&ensp;&ensp;
\ell&ensp;\text{\ell}&ensp;&ensp;
\neg&ensp;\text{\neg}&ensp;&ensp;\\
\top&ensp;\text{\top}&ensp;&ensp;
\flat&ensp;\text{\flat}&ensp;&ensp;
\natural&ensp;\text{\natural}&ensp;&ensp;
\sharp&ensp;\text{\sharp}&ensp;&ensp;
\wp&ensp;\text{\wp}&ensp;&ensp;\\
\bot&ensp;\text{\bot}&ensp;&ensp;
\clubsuit&ensp;\text{\clubsuit}&ensp;&ensp;
\diamondsuit&ensp;\text{\diamondsuit}&ensp;&ensp;
\heartsuit&ensp;\text{\heartsuit}&ensp;&ensp;
\spadesuit&ensp;\text{\spadesuit}&ensp;&ensp;\\
\mho&ensp;\text{\mho}^{a}&ensp;&ensp;
\Re&ensp;\text{\Re}&ensp;&ensp;
\Im&ensp;\text{\Im}&ensp;&ensp;
\angle&ensp;\text{\angle}&ensp;&ensp;
\partial&ensp;\text{\partial}&ensp;&ensp;\\$

##### <h2 id="7">特殊符号</h2>
>$\sum&ensp;\text{\sum}&ensp;&ensp;
\prod&ensp;\text{\prod}&ensp;&ensp;
\coprod&ensp;\text{\coprod}&ensp;&ensp;
\int&ensp;\text{\int}&ensp;&ensp;
\oint&ensp;\text{\oint}&ensp;&ensp;\\
\bigcap&ensp;\text{\bigcap}&ensp;&ensp;
\bigcup&ensp;\text{\bigcup}&ensp;&ensp;
\bigsqcup&ensp;\text{\bigsqcup}&ensp;&ensp;
\bigvee&ensp;\text{\bigvee}&ensp;&ensp;
\bigwedge&ensp;\text{\bigwedge}&ensp;&ensp;\\
\bigodot&ensp;\text{\bigodot}&ensp;&ensp;
\bigotimes&ensp;\text{\bigotimes}&ensp;&ensp;
\bigoplus&ensp;\text{\bigoplus}&ensp;&ensp;
\biguplus&ensp;\text{\biguplus}&ensp;&ensp;\\$

##### <h2 id="8">曲线函数</h2>
>$\text{\arccos}&ensp;\text{\cos}&ensp;&ensp;\text{\csc}&ensp;\text{\exp}&ensp;
\text{\ker}&ensp;\text{\limsup}&ensp;\text{\min}&ensp;\text{\sinh}&ensp;\\
\text{\arcsin}&ensp;\text{\cosh}&ensp;\text{\deg}&ensp;\text{\gcd}&ensp;
\text{\lg}&ensp;\text{\ln}&ensp;\text{\Pr}&ensp;\text{\sup}&ensp;\\
\text{\arctan}&ensp;\text{\cot}&ensp;\text{\det}&ensp;\text{\hom}&ensp;
\text{\lim}&ensp;\text{\log}&ensp;\text{\sec}&ensp;\text{\tan}&ensp;\\
\text{\arg}&ensp;\text{\coth}&ensp;\text{\dim}&ensp;\text{\inf}&ensp;
\text{\liminf}&ensp;\text{\max}&ensp;\text{\sin}&ensp;\text{\tanh}&ensp;\\$

##### <h2 id="9">分隔符号</h2>
>$\uparrow&ensp;\text{\uparrow}&ensp;&ensp;
\Uparrow&ensp;\text{\Uparrow}&ensp;&ensp;
\downarrow&ensp;\text{\downarrow}&ensp;&ensp;
\Downarrow&ensp;\text{\Downarrow}ensp;&ensp;
\{&ensp;\text{\{}&ensp;&ensp;\\
\}&ensp;\text{\}}&ensp;&ensp;
\updownarrow&ensp;\text{\updownarrow}&ensp;&ensp;
\Updownarrow&ensp;\text{\Updownarrow}ensp;&ensp;
\lfloor&ensp;\text{\lfloor}&ensp;&ensp;
\rfloor&ensp;\text{\rfloor}&ensp;&ensp;\\
\lceil&ensp;\text{\lceil}&ensp;&ensp;
\rceil&ensp;\text{\rceil}&ensp;&ensp;
\langle&ensp;\text{\langle}&ensp;&ensp;
\rangle&ensp;\text{\rangle}&ensp;&ensp;
/&ensp;\text{/}&ensp;&ensp;\\
\backslash&ensp;\text{\backslash}&ensp;&ensp;
|&ensp;\text{|}&ensp;&ensp;
\|&ensp;\text{\|}&ensp;&ensp;
\rmoustache&ensp;\text{\rmoustache}&ensp;&ensp;
\lmoustache&ensp;\text{\lmoustache}&ensp;&ensp;\\
\rgroup&ensp;\text{\rgroup}&ensp;&ensp;
\lgroup&ensp;\text{\lgroup}&ensp;&ensp;
\arrowvert&ensp;\text{\arrowvert}&ensp;&ensp;
\Arrowvert&ensp;\text{\Arrowvert}&ensp;&ensp;
\bracevert&ensp;\text{\bracevert}&ensp;&ensp;$

##### <h2 id="10">数学结构</h2>
>$\widetilde{abc}&ensp;\text{\widetilde{abc}}&ensp;&ensp;
\widehat{abc}&ensp;\text{\widehat{abc}}&ensp;&ensp;
\overleftarrow{abc}&ensp;\text{\overleftarrow{abc}}&ensp;&ensp;
\overrightarrow{abc}&ensp;\text{\overrightarrow{abc}}&ensp;&ensp;\\
\overline{abc}&ensp;\text{\overline{abc}}&ensp;&ensp;
\underline{abc}&ensp;\text{\underline{abc}}&ensp;&ensp;
\overbrace{abc}&ensp;\text{\overbrace{abc}}&ensp;&ensp;
\underbrace{abc}&ensp;\text{\underbrace{abc}}&ensp;&ensp;\\
\sqrt{abc}&ensp;\text{\sqrt{abc}}&ensp;&ensp;
\sqrt[n]{abc}&ensp;\text{\sqrt[n]{abc}}&ensp;&ensp;
f’&ensp;\text{f’}&ensp;&ensp;
\frac{abc}{xyz}&ensp;\text{\frac{abc}{xyz}}&ensp;&ensp;$

##### <h2 id="11">AMS希腊字母</h2>
>$\digamma&ensp;\text{\digamma}&ensp;&ensp;
\varkappa&ensp;\text{\varkappa}&ensp;&ensp;
\beth&ensp;\text{\beth}&ensp;&ensp;
\daleth&ensp;\text{\daleth}&ensp;&ensp;
\gimel&ensp;\text{\gimel}&ensp;&ensp;$

##### <h2 id="12">AMS分隔符号</h2>
>$\ulcorner&ensp;\text{\ulcorner}&ensp;&ensp;
\urcorner&ensp;\text{\urcorner}&ensp;&ensp;
\llcorner&ensp;\text{\llcorner}&ensp;&ensp;
\lrcorner&ensp;\text{\lrcorner}&ensp;&ensp;$

##### <h2 id="13">AMS箭头符号</h2>
>$\Rrightarrow&ensp;\text{\Rrightarrow}&ensp;&ensp;
\rightsquigarrow&ensp;\text{\rightsquigarrow}&ensp;&ensp;
\leftleftarrows&ensp;\text{\leftleftarrows}&ensp;&ensp;
\leftrightarrows&ensp;\text{\leftrightarrows}&ensp;&ensp;\\
\Lleftarrow&ensp;\text{\Lleftarrow}&ensp;&ensp;
\twoheadleftarrow&ensp;\text{\twoheadleftarrow}&ensp;&ensp;
\leftarrowtail&ensp;\text{\leftarrowtail}&ensp;&ensp;
\looparrowleft&ensp;\text{\looparrowleft}&ensp;&ensp;\\
\leftrightharpoons&ensp;\text{\leftrightharpoons}&ensp;&ensp;
\curvearrowleft&ensp;\text{\curvearrowleft}&ensp;&ensp;
\circlearrowleft&ensp;\text{\circlearrowleft}&ensp;&ensp;
\Lsh&ensp;\text{\Lsh}&ensp;&ensp;\\
\upuparrows&ensp;\text{\upuparrows}&ensp;&ensp;
\upharpoonleft&ensp;\text{\upharpoonleft}&ensp;&ensp;
\downharpoonleft&ensp;\text{\downharpoonleft}&ensp;&ensp;
\multimap&ensp;\text{\multimap}&ensp;&ensp;\\
\leftrightsquigarrow&ensp;\text{\leftrightsquigarrow}&ensp;&ensp;
\rightleftarrows&ensp;\text{\rightleftarrows}&ensp;&ensp;
\rightrightarrows&ensp;\text{\rightrightarrows}&ensp;&ensp;
\twoheadrightarrow&ensp;\text{\twoheadrightarrow}&ensp;&ensp;\\
\rightarrowtail&ensp;\text{\rightarrowtail}&ensp;&ensp;
\looparrowright&ensp;\text{\looparrowright}&ensp;&ensp;
\rightleftharpoons&ensp;\text{\rightleftharpoons}&ensp;&ensp;
\curvearrowright&ensp;\text{\curvearrowright}&ensp;&ensp;\\
\circlearrowright&ensp;\text{\circlearrowright}&ensp;&ensp;
\Rsh&ensp;\text{\Rsh}&ensp;&ensp;
\downdownarrows&ensp;\text{\downdownarrows}&ensp;&ensp;
\downharpoonright&ensp;\text{\downharpoonright}&ensp;&ensp;\\
\upharpoonright&ensp;\text{\upharpoonright}&ensp;&ensp;
\restriction&ensp;\text{\restriction}&ensp;&ensp;
\nleftarrow&ensp;\text{\nleftarrow}&ensp;&ensp;
\nrightarrow&ensp;\text{\nrightarrow}&ensp;&ensp;
\nLeftarrow&ensp;\text{\nLeftarrow}&ensp;&ensp;\\
\nRightarrow&ensp;\text{\nRightarrow}&ensp;&ensp;
\nleftrightarrow&ensp;\text{\nleftrightarrow}&ensp;&ensp;
\nLeftrightarrow&ensp;\text{\nLeftrightarrow}&ensp;&ensp;$

##### <h2 id="14">AMS二元关系符</h2>
>$\leqq&ensp;\text{\leqq}&ensp;&ensp;
\leqslant&ensp;\text{\leqslant}&ensp;&ensp;
\eqslantless&ensp;\text{\eqslantless}&ensp;&ensp;
\lesssim&ensp;\text{\lesssim}&ensp;&ensp;\\
\lessapprox&ensp;\text{\lessapprox}&ensp;&ensp;
\approxeq&ensp;\text{\approxeq}&ensp;&ensp;
\lessdot&ensp;\text{\lessdot}&ensp;&ensp;
\lll&ensp;\text{\lll,\llless}&ensp;&ensp;\\
\lessgtr&ensp;\text{\lessgtr}&ensp;&ensp;
\lesseqgtr&ensp;\text{\lesseqgtr}&ensp;&ensp;
\lesseqqgtr&ensp;\text{\lesseqqgtr}&ensp;&ensp;
\doteqdot&ensp;\text{\doteqdot,\Doteq}&ensp;&ensp;\\
\risingdotseq&ensp;\text{\risingdotseq}&ensp;&ensp;
\fallingdotseq&ensp;\text{\fallingdotseq}&ensp;&ensp;
\backsim&ensp;\text{\backsim}&ensp;&ensp;
\backsimeq&ensp;\text{\backsimeq}&ensp;&ensp;\\
\subseteqq&ensp;\text{\subseteqq}&ensp;&ensp;
\Subset&ensp;\text{\Subset}&ensp;&ensp;
\sqsubset&ensp;\text{\sqsubset}&ensp;&ensp;
\preccurlyeq&ensp;\text{\preccurlyeq}&ensp;&ensp;\\
\curlyeqprec&ensp;\text{\curlyeqprec}&ensp;&ensp;
\precsim&ensp;\text{\precsim}&ensp;&ensp;
\precapprox&ensp;\text{\precapprox}&ensp;&ensp;
\vartriangleleft&ensp;\text{\vartriangleleft}&ensp;&ensp;\\
\trianglelefteq&ensp;\text{\trianglelefteq}&ensp;&ensp;
\vDash&ensp;\text{\vDash}&ensp;&ensp;
\Vvdash&ensp;\text{\Vvdash}&ensp;&ensp;
\smallsmile&ensp;\text{\smallsmile}&ensp;&ensp;\\
\smallfrown&ensp;\text{\smallfrown}&ensp;&ensp;
\bumpeq&ensp;\text{\bumpeq}&ensp;&ensp;
\Bumpeq&ensp;\text{\Bumpeq}&ensp;&ensp;
\geqq&ensp;\text{\geqq}&ensp;&ensp;\\
\geqslant&ensp;\text{\geqslant}&ensp;&ensp;
\eqslantgtr&ensp;\text{\eqslantgtr}&ensp;&ensp;
\gtrsim&ensp;\text{\gtrsim}&ensp;&ensp;
\gtrapprox&ensp;\text{\gtrapprox}&ensp;&ensp;\\
\gtrdot&ensp;\text{\gtrdot}&ensp;&ensp;
\ggg&ensp;\text{\ggg,\gggtr}&ensp;&ensp;
\gtrless&ensp;\text{\gtrless}&ensp;&ensp;
\gtreqless&ensp;\text{\gtreqless}&ensp;&ensp;\\
\gtreqqless&ensp;\text{\gtreqqless}&ensp;&ensp;
\eqcirc&ensp;\text{\eqcirc}&ensp;&ensp;
\circeq&ensp;\text{\circeq}&ensp;&ensp;
\triangleq&ensp;\text{\triangleq}&ensp;&ensp;\\
\thicksim&ensp;\text{\thicksim}&ensp;&ensp;
\thickapprox&ensp;\text{\thickapprox}&ensp;&ensp;
\supseteqq&ensp;\text{\supseteqq}&ensp;&ensp;
\Supset&ensp;\text{\Supset}&ensp;&ensp;\\
\sqsupset&ensp;\text{\sqsupset}&ensp;&ensp;
\succcurlyeq&ensp;\text{\succcurlyeq}&ensp;&ensp;
\curlyeqsucc&ensp;\text{\curlyeqsucc}&ensp;&ensp;
\succsim&ensp;\text{\succsim}&ensp;&ensp;\\
\succapprox&ensp;\text{\succapprox}&ensp;&ensp;
\vartriangleright&ensp;\text{\vartriangleright}&ensp;&ensp;
\trianglerighteq&ensp;\text{\trianglerighteq}&ensp;&ensp;
\Vdash&ensp;\text{\Vdash}&ensp;&ensp;\\
\shortmid&ensp;\text{\shortmid}&ensp;&ensp;
\shortparallel&ensp;\text{\shortparallel}&ensp;&ensp;
\between&ensp;\text{\between}&ensp;&ensp;
\pitchfork&ensp;\text{\pitchfork}&ensp;&ensp;\\
\varpropto&ensp;\text{\varpropto}&ensp;&ensp;
\blacktriangleleft&ensp;\text{\blacktriangleleft}&ensp;&ensp;
\therefore&ensp;\text{\therefore}&ensp;&ensp;
\backepsilon&ensp;\text{\backepsilon}&ensp;&ensp;\\
\blacktriangleright&ensp;\text{\blacktriangleright}&ensp;&ensp;
\because&ensp;\text{\because}&ensp;&ensp;
\nless&ensp;\text{\nless}&ensp;&ensp;
\nleq&ensp;\text{\nleq}&ensp;&ensp;\\
\nleqslant&ensp;\text{\nleqslant}&ensp;&ensp;
\nleqq&ensp;\text{\nleqq}&ensp;&ensp;
\lneq&ensp;\text{\lneq}&ensp;&ensp;
\lneqq&ensp;\text{\lneqq}&ensp;&ensp;\\
\lvertneqq&ensp;\text{\lvertneqq}&ensp;&ensp;
\lnsim&ensp;\text{\lnsim}&ensp;&ensp;
\lnapprox&ensp;\text{\lnapprox}&ensp;&ensp;
\nprec&ensp;\text{\nprec}&ensp;&ensp;\\
\npreceq&ensp;\text{\npreceq}&ensp;&ensp;
\precnsim&ensp;\text{\precnsim}&ensp;&ensp;
\precnapprox&ensp;\text{\precnapprox}&ensp;&ensp;
\nsim&ensp;\text{\nsim}&ensp;&ensp;\\
\nshortmid&ensp;\text{\nshortmid}&ensp;&ensp;
\nmid&ensp;\text{\nmid}&ensp;&ensp;
\nvdash&ensp;\text{\nvdash}&ensp;&ensp;
\nvDash&ensp;\text{\nvDash}&ensp;&ensp;\\
\ntriangleleft&ensp;\text{\ntriangleleft}&ensp;&ensp;
\ntrianglelefteq&ensp;\text{\ntrianglelefteq}&ensp;&ensp;
\nsubseteq&ensp;\text{\nsubseteq}&ensp;&ensp;
\subsetneq&ensp;\text{\subsetneq}&ensp;&ensp;\\
\varsubsetneq&ensp;\text{\varsubsetneq}&ensp;&ensp;
\subsetneqq&ensp;\text{\subsetneqq}&ensp;&ensp;
\varsubsetneqq&ensp;\text{\varsubsetneqq}&ensp;&ensp;
\ngtr&ensp;\text{\ngtr}&ensp;&ensp;\\
\ngeq&ensp;\text{\ngeq}&ensp;&ensp;
\ngeqslant&ensp;\text{\ngeqslant}&ensp;&ensp;
\ngeqq&ensp;\text{\ngeqq}&ensp;&ensp;
\gneq&ensp;\text{\gneq}&ensp;&ensp;\\
\gneqq&ensp;\text{\gneqq}&ensp;&ensp;
\gvertneqq&ensp;\text{\gvertneqq}&ensp;&ensp;
\gnsim&ensp;\text{\gnsim}&ensp;&ensp;
\gnapprox&ensp;\text{\gnapprox}&ensp;&ensp;\\
\nsucc&ensp;\text{\nsucc}&ensp;&ensp;
\nsucceq&ensp;\text{\nsucceq}&ensp;&ensp;
\succnsim&ensp;\text{\succnsim}&ensp;&ensp;
\succnapprox&ensp;\text{\succnapprox}&ensp;&ensp;\\
\ncong&ensp;\text{\ncong}&ensp;&ensp;
\nshortparallel&ensp;\text{\nshortparallel}&ensp;&ensp;
\nparallel&ensp;\text{\nparallel}&ensp;&ensp;
\nvDash&ensp;\text{\nvDash}&ensp;&ensp;\\
\nVDash&ensp;\text{\nVDash}&ensp;&ensp;
\ntriangleright&ensp;\text{\ntriangleright}&ensp;&ensp;
\ntrianglerighteq&ensp;\text{\ntrianglerighteq}&ensp;&ensp;
\nsupseteq&ensp;\text{\nsupseteq}&ensp;&ensp;\\
\nsupseteqq&ensp;\text{\nsupseteqq}&ensp;&ensp;
\supsetneq&ensp;\text{\supsetneq}&ensp;&ensp;
\varsupsetneq&ensp;\text{\varsupsetneq}&ensp;&ensp;
\supsetneqq&ensp;\text{\supsetneqq}&ensp;&ensp;\\
\varsupsetneqq&ensp;\text{\varsupsetneqq}&ensp;&ensp;$

##### <h2 id="15">AMS二元操作符</h2>
>$\dotplus&ensp;\text{\dotplus}&ensp;&ensp;
\smallsetminus&ensp;\text{\smallsetminus}&ensp;&ensp;
\Cap&ensp;\text{\Cap,\doublecap}&ensp;&ensp;
\Cup&ensp;\text{\Cup,\doublecup}&ensp;&ensp;\\
\barwedge&ensp;\text{\barwedge}&ensp;&ensp;
\veebar&ensp;\text{\veebar}&ensp;&ensp;
\doublebarwedge&ensp;\text{\doublebarwedge}&ensp;&ensp;
\boxminus&ensp;\text{\boxminus}&ensp;&ensp;\\
\boxtimes&ensp;\text{\boxtimes}&ensp;&ensp;
\boxdot&ensp;\text{\boxdot}&ensp;&ensp;
\boxplus&ensp;\text{\boxplus}&ensp;&ensp;
\divideontimes&ensp;\text{\divideontimes}&ensp;&ensp;\\
\ltimes&ensp;\text{\ltimes}&ensp;&ensp;
\rtimes&ensp;\text{\rtimes}&ensp;&ensp;
\leftthreetimes&ensp;\text{\leftthreetimes}&ensp;&ensp;
\rightthreetimes&ensp;\text{\rightthreetimes}&ensp;&ensp;\\
\curlywedge&ensp;\text{\curlywedge}&ensp;&ensp;
\curlyvee&ensp;\text{\curlyvee}&ensp;&ensp;
\circleddash&ensp;\text{\circleddash}&ensp;&ensp;
\circledast&ensp;\text{\circledast}&ensp;&ensp;\\
\circledcirc&ensp;\text{\circledcirc}&ensp;&ensp;
\centerdot&ensp;\text{\centerdot}&ensp;&ensp;
\intercal&ensp;\text{\intercal}&ensp;&ensp;$

##### <h2 id="16">AMS杂类符号</h2>
>$\hbar&ensp;\text{\hbar}&ensp;&ensp;
\hslash&ensp;\text{\hslash}&ensp;&ensp;
\vartriangle&ensp;\text{\vartriangle}&ensp;&ensp;
\triangledown&ensp;\text{\triangledown}&ensp;&ensp;\\
\square&ensp;\text{\square}&ensp;&ensp;
\lozenge&ensp;\text{\lozenge}&ensp;&ensp;
\circledS&ensp;\text{\circledS}&ensp;&ensp;
\angle&ensp;\text{\angle}&ensp;&ensp;\\
\measuredangle&ensp;\text{\measuredangle}&ensp;&ensp;
\nexists&ensp;\text{\nexists}&ensp;&ensp;
\mho&ensp;\text{\mho}&ensp;&ensp;
\Finv&ensp;\text{\Finv}&ensp;&ensp;\\
\Game&ensp;\text{\Game}&ensp;&ensp;
\Bbbk&ensp;\text{\Bbbk}&ensp;&ensp;
\backprime&ensp;\text{\backprime}&ensp;&ensp;
\varnothing&ensp;\text{\varnothing}&ensp;&ensp;\\
\blacktriangle&ensp;\text{\blacktriangle}&ensp;&ensp;
\blacktriangledown&ensp;\text{\blacktriangledown}&ensp;&ensp;
\blacksquare&ensp;\text{\blacksquare}&ensp;&ensp;
\blacklozenge&ensp;\text{\blacklozenge}&ensp;&ensp;\\
\bigstar&ensp;\text{\bigstar}&ensp;&ensp;
\sphericalangle&ensp;\text{\sphericalangle}&ensp;&ensp;
\complement&ensp;\text{\complement}&ensp;&ensp;
\eth&ensp;\text{\eth}&ensp;&ensp;\\
\diagup&ensp;\text{\diagup}&ensp;&ensp;
\diagdown&ensp;\text{\diagdown}&ensp;&ensp;$
