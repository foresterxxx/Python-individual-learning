# Python个人学习笔记
个人学习Python的笔记（主要是给自己看的，顺手丢到github中）。笔者之前学C/C++，因此笔记中涉及到C/C++的部分语法比较区别（不影响实际阅读），另外由于个人能力有限，其中存在很多谬误与不准确，感谢读者指出，欢迎交流。
# 笔记目录（在笔记中添加[toc]即可建立可跳转的目录）
- [环境配置简述](#环境配置简述)
- [Python编程规范准则](#python编程规范准则)
- [前置](#前置)
- [安装管理Python扩展包（库）](#安装管理python扩展包库)
- [集成开发环境](#集成开发环境)
- [程序的打包与发布](#程序的打包与发布)
- [字面量](#字面量)
- [注释](#注释)
- [变量](#变量)
- [数据类型](#数据类型)
- [命名规范](#命名规范)
- [运算符](#运算符)
- [字符串相关](#字符串相关)
  - [1. 字符串定义](#1-字符串定义)
  - [2. 字符串拼接](#2-字符串拼接)
  - [3. 字符串格式化](#3-字符串格式化)
  - [4. 格式化精度控制](#4-格式化精度控制)
    - [4.1. 快速格式化](#41-快速格式化)
- [输入](#输入)
- [判断语句](#判断语句)
  - [5. if语句](#5-if语句)
  - [6. if-else语句](#6-if-else语句)
  - [7. if-elif-else语句](#7-if-elif-else语句)
  - [8. 实例](#8-实例)
- [循环语句](#循环语句)
  - [9. while语句](#9-while语句)
  - [10. for循环](#10-for循环)
    - [10.1. range语句](#101-range语句)
  - [11. break语句和continue语句](#11-break语句和continue语句)
- [函数](#函数)
- [杂项](#杂项)
- [数据容器](#数据容器)
  - [12. list列表](#12-list列表)
  - [13. 列表内置的方法](#13-列表内置的方法)
    - [13.1. 查询指定元素的下标](#131-查询指定元素的下标)
    - [13.2. 修改指定下标的元素值](#132-修改指定下标的元素值)
    - [13.3. 按位置插入值](#133-按位置插入值)
    - [13.4. 追加元素](#134-追加元素)
    - [13.5. 删除元素（按照索引删除）](#135-删除元素按照索引删除)
    - [13.6. 删除元素（按值删除）](#136-删除元素按值删除)
    - [13.7. 清空](#137-清空)
    - [13.8. 统计某元素的出现次数](#138-统计某元素的出现次数)
    - [13.9. 统计列表的长度](#139-统计列表的长度)
  - [14. tuple元组](#14-tuple元组)
  - [15. str字符串](#15-str字符串)
    - [15.1. 字符串替换](#151-字符串替换)
    - [15.2. 字符串分割](#152-字符串分割)
    - [15.3. 规整化处理/格式化处理](#153-规整化处理格式化处理)
  - [16. 序列与切片操作](#16-序列与切片操作)
  - [17. 集合set](#17-集合set)
    - [17.1. 添加新元素（按值）](#171-添加新元素按值)
    - [17.2. 移除元素](#172-移除元素)
    - [17.3. 随机弹出元素](#173-随机弹出元素)
    - [17.4. 清空](#174-清空)
    - [17.5. 取差集](#175-取差集)
    - [17.6. 消除差集](#176-消除差集)
    - [17.7. 取并集](#177-取并集)
    - [17.8. 统计元素个数](#178-统计元素个数)
  - [18. dict字典、映射](#18-dict字典映射)
    - [18.1. 新增（更新）元素](#181-新增更新元素)
    - [18.2. 删除元素](#182-删除元素)
    - [18.3. 统计元素（键值对）个数](#183-统计元素键值对个数)
    - [18.4. 清空字典](#184-清空字典)
    - [18.5. 获取全部的key](#185-获取全部的key)
  - [19. 总结](#19-总结)
  - [20. 数据容器的通用操作](#20-数据容器的通用操作)
- [函数进阶](#函数进阶)
  - [21. 多返回值](#21-多返回值)
  - [22. 传参调用方式](#22-传参调用方式)
  - [23. 匿名函数](#23-匿名函数)
    - [23.1. 函数作为参数传递](#231-函数作为参数传递)
    - [23.2. lambda匿名函数](#232-lambda匿名函数)
- [文件操作](#文件操作)
  - [24. 文件的打开读写关闭操作](#24-文件的打开读写关闭操作)
- [异常捕获](#异常捕获)
- [模块](#模块)
  - [25. 模块简述](#25-模块简述)
  - [26. \_\_main\_\_变量](#26-__main__变量)
  - [27. \_\_all\_\_变量](#27-__all__变量)
  - [28. 自定义Python包](#28-自定义python包)
- [实践专题——数据可视化](#实践专题数据可视化)
  - [29. Json简述](#29-json简述)
  - [30. pyecharts模块](#30-pyecharts模块)
