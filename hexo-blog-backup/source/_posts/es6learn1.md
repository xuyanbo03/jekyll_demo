---
title: ES6入门（一）
date: 2017-07-14
tags: [javascript]
categories: web前端
---

# ES6入门（一）


# let和const

- 不存在变量提升，一定在声明后使用

- let绑定所在代码块，存在暂时性死区，只有当let和const声明变量后，变量才可获取和使用

- 不允许在一个代码块重复声明

- const声明后要立即赋值

- const只保证变量指向的地址不变，不保证该地址的数据不变

<!-- more -->

# ES6六种声明变量的方法

- var
- function
- let
- const
- import
- class


- 跨模块变量使用export
- 全局变量和全局对象的属性
  - ES5中，全局变量==全局对象的属性
  - ES6中，let、const、class声明的全局变量不等于全局对象的属性
 

# 解构赋值

- 允许按照一定模式，从数组和对象中提取值，对变量进行赋值

- 使用圆括号：赋值语句的非模式部分可以使用

- 数组
  - 模式匹配：只要等号两边的模式相同，左边变量被赋予对应值
  - 不完全解构：等号左边的模式只匹配等号右边数组的一部分
  - 允许指定默认值
    - 严格等于undefined，默认值才生效
    - 设为null，默认值不会生效
    - 默认为表达式，惰性求值
    - 其他变量已赋值，默认值可为其他变量
    
- 对象
  - 变量必须与属性同名，先找到同名属性，再赋给对应的变量
  - 可用于嵌套结构的对象
  - 可指定默认值
    - 严格等于undefined，默认值才生效
    - 允许等号左边不放置任何变量名
    
- 字符串
  - 被转换成类似数组的对象
  
- 数值和布尔值
  - 先转换为对象
  
- 函数
  - 参数解构赋值
  
- 用途
  - 交换变量的值
  - 从函数返回多个值
  - 函数参数无次序的赋值
  - 函数参数默认值
  - 提取JSON数据（常用）
  - 遍历Map结构（常用）
  - 输入模块的指定（常用）