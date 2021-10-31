<font face="微软雅黑" size=8>

<h2>Emmet—写HTML/CSS快到飞起</h2>

Emmet语法，能大大提高代码书写。只需要敲一行代码就能生成你想要的完整HTML结构  

**1：html初始结构   **

**2：id（#）,class（.)**

>  id指令:# ; class指令:.  

- div#test  

  ```html
  <div id ="test">
      
  </div>
  ```

- div.test

  ```html
  <div class="test"><div>
  ```

  **3:子节点（>），兄弟节点（+），上级节点（^）**

- div>ul>li>p

  ```html
  <div>
      <ul>
          <li>
              <p>
                  
              </p>
          </li>
      </ul>
  </div>
  ```

- div+ul+p

  ```html
  <div></div>
  <ul></ul>
  <p></p>
  
  ```

- div>ul>li^div(这里的`^`是接在`li`后面所以在`li`的上一级，与`ul`成了兄弟关系,当然两个^^就是上上级）

  ```html
  <div>
      <ul>
          <li></li>
      </ul>
      <div></div>
  </div>
  ```

**   4:重复**

- li*5

  ```html
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  ```

  

**5：分组（()）**

- div>(ul>li>a)+div>p

  > **括号里面的内容为一个代码块，表示与括号内部嵌套和外面的的层级无关**）  

```html
<div>
    <ul>
        <li><a href="#">hh</a></li>
    </ul>
    <div>
        <p></p>
    </div>
</div>
```

**6：属性（[attr]）——id，class都有怎么能少了属性呢**

- a[href=’###’ name=‘xiaoA’] （**中括号内填写属性键值对的形式，并且空格隔开

  ```html
  <a href="###" name="xx">hh</a>
  ```

**7:编号（$）**

- ul>li.test$*3 （**$代表一位数，后面更上\*数字就代表从1递增到填写的数字**）

  ```html
  <ul>
      <li class="text1"></li>
      <li class="text2"></li>
      <li class="text3"></li>
  </ul>
  ```

  > 如果想自定义从几开始递增的话就利用：$@+数字*数字 ( 例如：ul>li.test$@3*3)

```html
<ul>
    <li class="text3"></li>
    <li class="text4"></li>
    <li class="text5"></li>
</ul>
```

**8:文本（{}）**

> 文本指令：{}

- ul>li.test$*3{测试$} （**{里面填写内容，可以和$一起组合使用哦}**）

```html
<ul>
    
    <li class="test1">测试1</li>
    <li class="test2">测试1</li>
    <li class="test3">测试1</li>
</ul>
```

**9：隐藏标签**

> 这个标签没有指令，而是部分标签可以不使用输入标签，直接输入指令，即可识别父类标签。

- **默认div** 例如：`.test`

- **li**： 可在ul 和 ol 中使用 例如：`ul>.test$*3`

  ```html
  <ul>
     <li class="test1"></li>
     <li class="test2"></li>
     <li class="test3"></li>
   </ul>
  ```

  

- **option**：可在select中使用例如：`select>.test$*5`

- **tr**：可在 table、tbody、thead 和 tfoot 中使用

- **td**：可在 tr 中使用

