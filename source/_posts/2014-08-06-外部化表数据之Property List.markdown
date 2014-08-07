---
layout: post
title: "外部化表数据之Property List"
date: 2014-08-06 20:48
comments: true
categories: 学习
---
将静态数据从代码中分离出来是一个很好的做法。
假设让需要添加100多个新数据到应用程序中,需要返回源代码,将新的数据添加到初始化代码中，这无疑使得代码看起来表冗长。同时编辑这些代码并不简单,并且必须要严格遵守Objective-C语法，更改代码可能会引入其他错误。最好是将数据和代码逻辑分离。
Property List 提供了一个方便的方法来存放简单的结构数据,通常为XML格式。但是不能使用Property List 存放所有类型的数据。
下面开始转换数据为 Property List：
首先创建一个空的Property List 文件。
其次在Property List中添加n个数据数组，并添加完成了所有数组元素。
最后Property List中读取内容相当简单iOS SDK已经有内置的方法来处理该文件的读写操作。
Property List并不是存放表数据的最好方法，还有很多其他方法。