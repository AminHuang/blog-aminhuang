---
layout: post
title:  "DOM与BOM"
date:   2015-03-20 16:14:00
---
回顾基础知识。

DOM
------

DOM, Document Object Model, 文档对象模型，是针对XML但被经过扩展用于HTML的应用程序编程接口(API, Application Programming Interface)。   
DOM把整个页面映射成一个多层节点结构。   
通过DOM创建表示整个文档的树形图，开发人员获得了控制页面内容和结构的主动权，借助DOM提供的API，开发人员可以轻松自如地删除、添加、替换或修改任何节点。

   

### DOM级别     

#### DOM1级   
DOM1级由两个模块组成：*DOM核心(DOM Core)*和*DOM HTML*。   
DOM核心规定的是如何映射基于XML的文档结构，以便简化对文档中任意部分的访问和操作。   
DOM HTML模块在DOM核心的基础上加以扩展，添加了对HTML的对象和方法。 

#### DOM2级   
DOM2级在原来DOM基础上又扩充了鼠标和用户界面事件、范围、遍历（迭代DOM文档的方法）等细分模块，而且通过对象接口增加了对CSS的支持。   
DOM2级引入了下列新模块，也给出了众多新类型和新接口的定义。   
*   DOM视图(DOM Views):定义了跟踪不同文档（例如，应用CSS之前和之后的文档）视图的接口   
*   DOM事件(DOM Events):定义了事件好事件处理的接口   
*   DOM样式(DOM Style):定义了基于CSS为元素应用样式的接口   
*   DOM遍历和范围(DOM Traersal and Range):定义了遍历和操作文档树的接口   

#### DOM3级   
DOM加载和保存(DOM Load and Save)    模块：引入了以统一方式加载和保存文档的方法   
DOM验证(DOM Validation)模块：新增了验证文档的方法     
DOM3级也对DOM核心进行了扩展，开始支持XML1.0的标准   


BOM
--------

BOM, Brower Object Model, 浏览器对象模型，可访问和操作浏览器窗口。   
没有BOM标准可以遵循，因此每个浏览器都有自己的实现。




