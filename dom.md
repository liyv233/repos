<h2> DOM </h2>

js是一门脚本语言，读一行执行一行。

<h4>浏览器执行js 简介</h4>

- 浏览器分为两部分，**渲染引擎（内核）和js引擎**



<h4>dom</h4>

- dom  简介

> dom 是处理页面，文档的 标准 编程接口
>
> 作用：改变页面中的内容，结构和样式

- 文档

> 一个页面就是一个文档，DOM里面用 document 表示

![image-20211106174811183](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106174811183.png)

- 元素

  > 页面中所有的标签都是元素，DOM中用 element 表示 

- 节点

> 网页中所有的内容都是节点（标签，属性，文本，注释等），DOM中 用  node 表示

**DOM把以上内容都看做是对象**



<h4>获取元素</h4>

方法：

- 根据  ID  获取

- 

  ​            **   getElementByid()**

  ![image-20211106180003410](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106180003410.png)

- 

![image-20211106180652923](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106180652923.png)



![image-20211106182606773](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106182606773.png)



- 根据标签名获取



![image-20211106184700181](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106184700181.png)

![image-20211106185507595](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106185507595.png)



- 通过HTML5 新增方法获取 （i9以上版本支持html5）



![image-20211106193635415](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106193635415.png)

![image-20211106193505097](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106193505097.png)



- 特殊元素获取

![image-20211106203435814](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106203435814.png)

<h4>事件</h4>

- 事件概述

![image-20211106203804138](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106203804138.png)

- 事件组成

![image-20211106204640548](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106204640548.png)



- 执行事件的步骤

![image-20211106205437266](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106205437266.png)

- 鼠标事件



![image-20211106205502664](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211106205502664.png)



- 操作元素

![image-20211108082742450](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108082742450.png)





![image-20211108091203695](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108091203695.png)





![image-20211108091221933](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108091221933.png)



- innerText 和 innerHTML 的区别



![image-20211108091445651](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108091445651.png)



- **常用元素的属性操作**

![image-20211108091552132](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108091552132.png)

![image-20211108091624811](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108091624811.png)



![image-20211108131642133](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108131642133.png)





![image-20211108131647036](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108131647036.png)



- **表单元素的属性操作**

  ![image-20211108134004720](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108134004720.png)

![image-20211108133857596](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211108133857596.png)



- 对时间

![image-20211110082801177](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110082801177.png)



- 操作元素--修改样式属性

![image-20211110130334260](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110130334260.png)

- 当样式较少或者功能简单的时候用style

![image-20211110130419877](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110130419877.png)



![image-20211110131125444](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110131125444.png)



- 当样式复杂时，现在css中写好类名，再在函数中引用  className

![image-20211110154827515](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110154827515.png)

![image-20211110154339307](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110154339307.png)



- 循环精灵图

![image-20211110131819407](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110131819407.png)

![image-20211110132415463](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110132415463.png)

![image-20211110154835703](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110154835703.png)



- **事件---失去（onblur)与得到(onfocus)焦点**



![image-20211110133535209](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110133535209.png)



![image-20211110160132909](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110160132909.png)





<h4>算法--排他思想</h4>



![image-20211110184731867](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110184731867.png)





![image-20211110184742699](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110184742699.png)



![image-20211110185722155](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110185722155.png)



- **鼠标经过和鼠标离开事件**

![image-20211110185939986](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110185939986.png)

![image-20211110190522138](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211110190522138.png)





- **自定义属性的操作**

> 1：得到属性的两种方法：

![image-20211111175541912](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111175541912.png)

![image-20211111175401146](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111175401146.png)



> 2:  设置元素属性值



<img src="C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111180202196.png" alt="image-20211111180202196" style="zoom: 67%;" />

![image-20211111180110792](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111180110792.png)



![image-20211111180317367](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111180317367.png)



- h5新增的获取自定义属性的方法：

> 兼容性较差（仅支持11及以上版本），开发不常用



![image-20211111205152800](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111205152800.png)





- **DOM 重点 核心**



![image-20211113215404965](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215404965.png)

![image-20211113215425122](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215425122.png)

![image-20211113215502894](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215502894.png)

![image-20211113215511479](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215511479.png)

![image-20211113215612137](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215612137.png)



![image-20211113215945846](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113215945846.png)



![image-20211113220002469](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211113220002469.png)







<h4>高级事件</h4>



- 注册事件

![image-20211114120552339](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114120552339.png)



- 方法监听注册事件

  

![image-20211114120715601](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114120715601.png)

![image-20211114121021774](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114121021774.png)

- attachEvent (了解)

![image-20211114121638829](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114121638829.png)



- 删除事件（解绑事件）

![image-20211114122104161](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114122104161.png)

![image-20211114122401397](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114122401397.png)





- **DOM 事件流**

![image-20211114123202464](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114123202464.png)

![image-20211114124643691](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114124643691.png)





- **事件对象**

  ​									![image-20211114125911654](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114125911654.png)  									

  

  ![	](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114125929703.png)

  

![image-20211114125556102](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114125556102.png)

- 解决兼容性处理

![image-20211114125646934](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114125646934.png)



- 事件对象的常用属性和方法

![image-20211114145131686](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114145131686.png)

![image-20211114145626730](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114145626730.png)



- 阻止默认行为（事件） ：让链接不跳转或者按钮不提交等

![image-20211114150708923](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114150708923.png)

![image-20211114150729744](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114150729744.png)



- **阻止冒泡**

![image-20211114152729498](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114152729498.png)

![image-20211114152739773](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114152739773.png)

![image-20211114152805650](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114152805650.png)



- 事件委托（代理，委派）

![image-20211114155809453](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114155809453.png)

![image-20211114155821012](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114155821012.png)



- 鼠标事件-- 禁止鼠标右键菜单

![image-20211114160216870](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114160216870.png)

![image-20211114160154203](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114160154203.png)

![image-20211114160306648](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114160306648.png)



- 鼠标事件

![image-20211114161619665](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114161619665.png)



- **常用键盘事件**

![image-20211114163505614](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114163505614.png)



![image-20211114163423183](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114163423183.png)



- 键盘事件的对象

![image-20211114170755975](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114170755975.png)



![image-20211114170806829](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114170806829.png)































































