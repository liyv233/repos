<h2> 案例 </h2>

- ***密码框的眼睛和tab 栏切换 ***

![image-20211111203917972](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111203917972.png)

```html
<style>
        * {
            margin: 0;
            padding: 0;
        }
        li {
            list-style: none;
        }
        body {
            background-color: #f3f5f7;
        }
      #jd {
          position: relative;
          margin: 100px auto;
         background-color: #fff;
          width: 400px;
          border-bottom: 1px solid black;
      }
      #jd1 {
          position: absolute;
          margin-top: 8px;
          right: 1px;
          width: 24px;
         
      }
      #jd input {
        height: 30px;
        width: 370px;
        border: 0px;
        outline: none;
        height: 40px;
      }
     .tab {
         width: 1288px;
         height: 596px;
         
     }
     .tab .tab_head {
         height: 58px;
        background-color:rgb(117, 112, 112);
     }
     .tab_head ul li {
         float: left;
         padding: 0 20px;
         
         font-size: 18px;
        line-height: 58px;
     }
     .tab_head ul li:hover {
        background-color: rgb(250, 134, 88);
     }
     .tab .tab_body div {
        display: none;
     }
     .cg_color {
         background-color: rgba(248, 60, 12, 0.925);
     }
    </style>
</head>
<body>
    <div id="jd">
        <input type="password" id="psd">
        <label for="jd1"><img src="js-images/第一天/close.png" alt="" id="jd1"></label>
    </div>
       <script>
           var psd=document.getElementById('psd');
           var jd1=document.getElementById('jd1');
           var temp=1;
           jd1.onclick=function() {
               if(temp==1)
                 {
                    psd.type='test';
                    jd1.src='js-images/第一天/open.png';
                     temp=0;
                } 
                else {
                    psd.type='password';
                    jd1.src='js-images/第一天/close.png';
                     temp=1;
                }
           }
       </script>

       <div class="tab">
           <div class="tab_head">
               <ul>
                   <li>商品介绍</li>
                   <li>规格与包装</li>
                   <li>售后保障</li>
                   <li>商品评价（50000）</li>
                   <li>手机社区</li>
               </ul>
           </div>
           <div class="tab_body">
               <div style="display: block;" class="items">商品介绍</div>
               <div class="items" >规格与包装</div>
               <div class="items" >售后保障</div>
               <div class="items" >商品评价内容</div>
               <div class="items" >手机社区</div>
           </div>
       </div>
       <!-- 点击变色，排他思想 -->
       <script>
        //    1：获取元素
        var tab_head = document.querySelector('.tab_head');
        var lis = tab_head.querySelectorAll('li');
        var items=document.querySelectorAll('.items');
        // 2:for 循环，绑定点击事件
        for (var i=0;i<lis.length;i++) {

            // 设置自定义属性，作为索引号
            lis[i].setAttribute('index',i);
            lis[i].onclick=function() {
                 // 干掉所有人，其余的li清除 class 这个类
                for(var i=0;i<lis.length;i++ ) {
                    lis[i].className='';
                }
                this.className='cg_color';
                // 3：下面的显示内容模块，一一对应，排他
               var index= this.getAttribute('index');
               for(var j=0;j<items.length;j++) {
                   items[j].style.display='none';
               }
               
               items[index].style.display='block';
            }
                

        }
       </script>
```



- 节点操作---下拉菜单



- 基本布局

![image-20211111214820954](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111214820954.png)



![image-20211111215238488](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111215238488.png)



- 节点操作---简单留言发布

![image-20211111221321108](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111221321108.png)

![image-20211111222040124](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211111222040124.png)



- 节点操作----删除留言

![image-20211112190138008](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112190138008.png)

--- 添加a：

![image-20211112190202164](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112190202164.png)

![image-20211112190246725](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112190246725.png)



- 动态生成表格 

![image-20211112191843595](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112191843595.png)

- 遍历对象



![image-20211112193809755](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112193809755.png)



--创建行

![image-20211112194007248](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112194007248.png)



--创建单元格并单元格得到内容

![image-20211112194041302](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112194041302.png)



--  删除操作

![image-20211112194426059](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112194426059.png)



![image-20211112195045946](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211112195045946.png)





- 鼠标天使（案例分析）

![image-20211114162050409](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114162050409.png)

![image-20211114162715262](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114162715262.png)



- 键盘事件----快递单号查询

![image-20211114172622226](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114172622226.png)

![image-20211114172218358](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114172218358.png)

![image-20211114172751498](C:\Users\红烧的咸鱼酱\AppData\Roaming\Typora\typora-user-images\image-20211114172751498.png)











