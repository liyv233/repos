<h2>背景</h2>

<h4>1：背景颜色</h4>

> 背景颜色：background-color:  color  ; ( 默认为 transparent，透明的   )
>
> **背景颜色半透明**
>
> > background :rgba (0,0,0,0.6);（第四个参数为透明度，取值范围为0~1；
> >
> > 只会使盒子背景色半透明，盒子内容不会有影响


<h4>2：背景图片</h4>

> background-image : 该属性描述了背景图像，实际开发中常见于logo或者一些装饰性的小图片或者是超大的背景图片，优点是非常便于控制位置（精灵图也是一种运用场景）
>
> 语法格式： background-image : none(默认）| url （） ；

```html
<style>
    div {
        width: 250px;
        height :250px;
        background-image :url(images/images/women.jpg);
        background-repeat: no-repeat;
        background-color:  pink  ;    
        background-position: center top;
    }
</style>
<div>
    
</div>
```

- 背景图片铺满盒子（背景平铺），

- 可以用background-repeat:  repeat(默认平铺) | no-repeat |  repeat-x（沿着x轴平铺） repeat-y ;（沿着y轴平铺）

  |背景图片会压住背景颜色

<h3>背景图片位置</h3>

>可以改变图片在背景中的位置
>
>语法格式：  background-position :  x  y  ;
>
>参数代表坐标：x坐标和y坐标，可以用方位名词或者精确单位
>
>> 方位名词：position：top|center|botton|left|right
>>
>> > 如果指定两个值都是方位名词，则两个值前后顺序无关，如：left top ==top left
>> >
>> > 如果只指定了一个方位名词，另外一个省略，则第二个值默认居中对齐
>>
>> 精确单位：  百分数| 由浮点数字和单位标识符组成的长度(x y 位置不能调换)，只指定一个数值，则一定是x值，y轴默认居中
>>
>> 混合单位：方位单位和精确单位混合使用  x y 顺序一定

方位名词的应用：超级无敌精简版的签到 logo，什么时候才能做一个完整版的呢？冲鸭！！！

```html
<style>
    *{
            padding: 0;
            margin: 0 auto;
        }
        .test {
            background-color:rgb(144, 202, 249);
            height: 64px;
        }
       
         .logo {
            width: 200px;
            height: 60px;
            background-image: url(images/科协logo1-1-1.jpg);
            display: inline-block;
            background-position: 20px;
            background-repeat: no-repeat;
            font-size: 20px;
            color: #ffffff;
            line-height: 60px;
            text-indent: 65px;
        }
       
    </style>
</head>
<body>
    <div class="test">
        
        <div class="logo">三院科协</div>
    </div>
</body>
```

插入背景图片(水平居中，距离顶部有40px距离, 固定背景图像)

```html
 <style>
        body {
            background-image: url(images/背景.jpg);
            background-repeat: no-repeat;
            background-position: center 40px;
            font-size :20px;
            color : pink ;
            background-attachment : fixed;
        }
    </style>
</head>
<body>
    <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p> 
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
     <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
    <p>好想好想好想好想喝奶茶</p>
   
</body>
```

<h4>背景图像的固定(背景附着)</h4>

> background-attachment 属性设置背景图像是否固定或者随着页面的其余部分滚动
>
> 常用来制作视差滚动的效果
>
> background-attachment: scroll  (默认滚动)| fixed（固定的）

- **背景的复合写法**

  > 没有特定的顺序，但习惯性顺序为：background-color : ;  background-image : ; background-repeat : ; 
  >
  >  background-attachment :  ;  background-position : ;

```html
 url(images/背景.jpg);  no-repeat; fixed; center 40px;
```

