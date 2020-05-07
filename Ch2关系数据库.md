![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge0km91dxcj30sh0feqen.jpg)

# 1.关系模型概述

## 1.1概述

1. 关系数据库系统

   ==是支持关系模型的数据库系统==

2. 关系模型的组成

   + 关系数据结构
   + 关系操作集合
   + 关系完整性约束



## 1.2关系数据结构

1. 单一的数据结构--***<u>关系</u>***

   现实世界的实体以及实体间的各种联系均用关系来表示

2. 数据的逻辑结构--***<u>二维表</u>***

   从用户角度，关系模型中数据的逻辑结构是一张二维表



## 1.3关系操作集合

### 1.3.1常用的关系操作



1. 查询

   选择、投影、连接、除、并、交、差

2. 数据更新

   插入、删除、修改

3. 查询的表达能力是其中最主要的部分



### 1.3.2关系操作的特点



==集合操作方式，即操作的对象和结果都是集合！！==

+ 关系数据模型的数据操作方式：一次一集合
+ 非关系数据模型的数据操作方式：一次一记录



### 1.3.3关系数据语言的种类



1. ***<u>关系代数语言</u>***

2. ***<u>关系演算语言：</u>***用谓词来表达查询要求

   + 元组关系演算语言

     谓词变元的基本对象是元组变量，比如APLHA，QUEL

   + 域关系演算语言

     谓词变元的基本对象是域变量，比如QBE

3. 具有关系代数和关系演算双重特点的语言

   典型代表--==SQL==



### 1.3.4关系数据语言的特点



1. 关系语言是一种高度非过程化的语言
   + 存取路径的选择由DBMS的优化机制来完成
   + 用户不必用循环结构就可以完成数据操作
2. 能够嵌入高级语言中使用
3. 关系代数、元组关系演算和域关系演算三种语言在表达能力上完全等价！



## 1.4关系的完整性约束

1. ***<u>实体完整性</u>***

   通常由关系系统自动支持

2. ***<u>参照完整性</u>***

   早期系统不支持，目前大型系统能自动支持

3. ***<u>用户定义的完整性</u>***

   + 反映应用领域需要遵循的约束条件，体现了具体领域中的语义约束
   + 用户定义后由系统支持

# 2.关系数据结构

关系模型建立在集合代数的基础上

关系数据结构的基本概念

+ 关系
+ 关系模式
+ 关系数据库



## 2.1关系

### 2.1.1域(Domain)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0loe81i8j30qv0gjalk.jpg)

### 2.1.2笛卡尔积(Cartesian Product)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0lu1b3ymj30uk0hb166.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0lu6m89wj30s70f2dqp.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0lua18pwj30s50fzn8o.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0lv1yv26j30tw0bw7dc.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0lv501mnj30qx0i47h1.jpg)



### 2.1.3关系(Relation)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0m9aoy38j30sv0cak0d.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge0mcuozpjj30s70hck40.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0mcz2l46j30s30gtam8.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge0mek9ztyj30s70br117.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0meo07dpj30t90fln96.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge0mesjn82j30sm0dbtik.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0mf0o28rj30pv0gjal7.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge0mf4evodj30ik0gaai6.jpg)



## 2.2关系模式

### 2.2.1什么是关系模式

1. 关系模式(Relation Schema)是==型==

   关系是==值==

2. ***<u>关系模式是对关系的描述</u>***



### 2.2.2定义关系模式

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0mkc7wfqj30ml0gjajz.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0mkhp1itj30rb0g3qe8.jpg)



### 2.2.3关系模式与关系

1. 关系模式

   对关系的描述，是静态的、稳定的

2. 关系

   关系模式在某一时刻的状态或内容

   是动态的、随时间不断变化的

3. 关系和关系模式往往统称为关系，通过上下文加以区别



## 2.3关系数据库



![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0mogq8u9j30tu0hq7h8.jpg)

关系数据库的值简称为关系数据库RDB！！！

# 3.关系的完整性

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0mw3vmxgj30tl0gf4bf.jpg)



## 3.1实体完整性

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge0mzbi133j30mn0d8n4z.jpg)



## 3.2参照完整性

### 3.2.1关系间的引用

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge0n4nvm7fj30ou0emajs.jpg)

### 3.2.2外码

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0n7gg4ovj30u10awwnm.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0n7kb27dj30pd08g0yf.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0n9ri3osj30tp0d4wnz.jpg)



### 3.2.3参照完整性规则

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge0ncngu33j30ow0dpdp4.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge0nctwm95j30sm0fln8z.jpg)



## 3.3用户定义的完整性

1. ==用户定义的完整性是针对某一具体关系数据库的约束条件，反映某一具体应用所涉及的数据必须满足的语义要求。==
2. 关系模型提供定义和检验这类完整性的机制，以便用统一的系统的方法来处理它们，而不要由应用程序承担这一功能。

# 4.关系代数

## 4.1概述

### 4.1.1关系代数

1. 一种抽象的==查询==语言。
2. 用***<u>对关系的运算</u>***来表达查询。(???==说实话没看懂==???)

### 4.1.2运算的三要素

1. 运算对象：关系
2. 运算结果：关系
3. 运算符：四类



运算符

1. ***<u>集合运算符</u>***

   + 将关系看成元组的集合
   + 运算是从关系的“水平”方向即行的角度来进行

2. ***<u>专门的关系运算符</u>***

   不仅涉及行而且设计列

3. ***<u>算术比较符</u>***

   辅助专门的关系运算符进行操作

4. ***<u>逻辑运算符</u>***

   辅助专门的关系运算符进行操作



![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge14e2ag4bj30o50frdpw.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge14ecppnjj30oz0e5guq.jpg)

## 4.2传统的集合运算

### 4.2.1并

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge14l951x8j30on0f0qca.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge14lqpddzj30sf0hzna4.jpg)



### 4.2.2差

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge14rr9xh6j30q70em7dw.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge14rzurgkj30sf0itk4t.jpg)



### 4.2.3交

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge14sw207kj30pi0fin75.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge14t0c595j30st0i6gyu.jpg)



### 4.2.4广义笛卡尔积

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge14usyz60j30r60gkqek.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge14v0x6c4j30s00ir16p.jpg)



## 4.3专门的关系运算

### 4.3.1选择

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge1534kwwxj30s70hiws1.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge15397536j30ou0cajyl.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge153fiknuj30sa0hjqcf.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge153nxyeqj30q30ee0xu.jpg)



### 4.3.2投影

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge157bk7bqj30mw09xdlq.jpg)

![img](https://wx1.sinaimg.cn/mw690/005LasY6gy1ge157kp3xmj30ts0eq13x.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge157oi5mjj30r90ddthx.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge157spzuzj30kb0fpwmb.jpg)

### 4.3.3连接

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge15dkmn4dj30sc0h5wrn.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge15e8cvuqj30so0eqqe4.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge15egpyktj30rb0evwp9.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge15ekxlccj30ru0gvk2u.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge15ep43v9j30qn0id14p.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge15etwul3j30o50i4dqm.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge15eyodnhj30nv0hswox.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge15f5owjfj30ky0hzdp1.jpg)



### 4.3.4除

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge169mwxgej30sq0hgqg8.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge169ugf22j30p40gjgvm.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge16a1eygij30ri0hgk3c.jpg)

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge16a6h2vdj30sf0grqfd.jpg)

![img](https://wx3.sinaimg.cn/mw690/005LasY6gy1ge16agf4v0j30qc0hsaln.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge16akz7pwj30on0hpwpb.jpg)





## 4.4小结

1. ***<u>关系代数运算</u>***

   并、差、交、广义笛卡尔积、投影、选择、连接、除

2. ***<u>基本运算</u>***

   并、差、广义笛卡尔积、投影、选择

3. ***<u>交、连接、除</u>***

   + 可以用五种基本运算来表达
   + 引进它们并不增加语言的能力，但可以简化表达

![img](https://wx2.sinaimg.cn/mw690/005LasY6gy1ge16pct238j30sc0dnqcx.jpg)

![img](https://wx4.sinaimg.cn/mw690/005LasY6gy1ge16vtrsqhj30sf0gq7gs.jpg)

# 5.关系演算

