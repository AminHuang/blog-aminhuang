---
layout: post
title:  "CSS3创建一个旋转可变色按钮"
date:   2015-03-13 15:17:00
---
html代码:
{% highlight html %}
<div>
    <a class="button">旋转按钮</a>
</div>
{% endhighlight %}

css代码:
{% highlight css %}
.button {
    background: #aaa;
    color: #555;
    font-weight: bold;
    font-size: 15px;
    padding: 10px 15px;
    border:none;
    margin:50px;
    cursor:pointer; 

    -webkit-transition: -webkit-transform 1s, opacity 1s background 1s, width 1s, height 1s, font-size 1s;

    -o-transition-property: width, height, -o-transform, background, font-size, opacity, color;
    -o-transition-duration:1s, 1s, 1s, 1s, 1s, 1s, 1s;

    -moz-transition-property: width, height, -moz-transform, background, font-size, opacity, color;
    -moz-transition-duration: 1s, 1s, 1s, 1s, 1s, 1s, 1s;

    transition-property: width, height, transform, background, font-size, opacity;
    transition-duration: 1s, 1s, 1s, 1s, 1s, 1s;

    -webkit-border-radius: 5px;
    border-radius:  5px;

    box-shadow:  0 0 2px rgba(0,0,0,0.5);

    text-shadow: 0 0 5px rgba(255, 255, 255, 0.5);

    display: inline-block;
}

{% endhighlight %}

上面代码用来转换属性，它可以定义转换宽度，高度，背景，颜色，透明度等等。
在这里定义了过渡时间为1s。

下面，定义鼠标悬浮时候产生的效果。

{% highlight css %}
.button:hover {
    -moz-transform: rotate(360deg);
    -webkit-transform: rotate(360deg);
    -o-transform: rotate(360deg);
    transform: rotate(360deg);

    background: #99a411;
    font-size: 30px;
    color: #fff;
}

{% endhighlight %}

旋转360度，其余代码是更改颜色，字体大小，颜色。

效果：
<link rel="stylesheet" href="{{ "/static/css/post_20150313.css" | prepend: site.baseurl }}">
<div>
    <a class="button">旋转按钮</a>
</div>

附上过渡属性列表：
<div>
<table>
<tbody>
<tr> 
<th style="width:30%;">属性</th> <th>描述</th> <th style="width:5%;">CSS</th> 
</tr>
<tr> 
<td>transition</td>
<td>简写属性，用于在一个属性中设置四个过渡属性。</td> 
<td>3</td> 
</tr>
<tr> <td>transition-property</td> <td>规定应用过渡的 CSS 属性的名称。</td> <td>3</td> 
</tr> 
<tr> <td>transition-duration</td> <td>定义过渡效果花费的时间。默认是 0。</td> <td>3</td> </tr> 
<tr> <td>transition-timing-function</td> <td>规定过渡效果的时间曲线。默认是 "ease"。</td> <td>3</td> </tr> 
<tr> <td>transition-delay</td> <td>规定过渡效果何时开始。默认是 0。</td> <td>3</td> </tr> 
</tbody>
</table>
</div>