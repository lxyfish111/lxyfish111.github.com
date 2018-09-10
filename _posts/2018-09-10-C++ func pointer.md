---
layout: post
category: ""
title:  "c++ func pointer"
tags: [c++]
---



函数名可以作为函数的地址，但这是有前提条件的，从函数到指针的隐式转换是函数名在表达式中的行为，这个转换仅在表达式中才会发生，这只是函数名众多性质中的一个，而非本质，函数名的本质是函数实体的代表。

对于C++，规定非静态成员函数的左值不可获得，因此非静态成员函数不存在隐式左值转换，即不存在像常规函数那样的从函数到指针的隐式转换，所以必须在非静态成员函数前使用&操作符才能获得地址。
