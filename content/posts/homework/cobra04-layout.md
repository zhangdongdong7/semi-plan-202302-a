---
title: "cobra04 - 项目工程目录结构（简单）"
subtitle: "Cobra Layout"
categories:
  - 半月刊
tags:
  - 半月刊202302A
  - 简单
date: "2023-01-16T22:34:14+08:00"
lastmod: "2023-01-16T22:34:14+08:00"
toc: true
draft: false
hiddenFromHomePage: false
pinTop: true
---



# Cobra04 - 项目工程目录结构（简单）

## 提示

阅读 [golang项目结构](https://github.com/golang-standards/project-layout) 

## 作业要求

1. 将 [作业: cobra - 01 实现编译与参数绑定](https://www.devopscamp.cc/semi-plan-202301-2/posts/homework/cobra01/) 进行改造， 改造完成后符合工程目录

**参考建议**

```bash
$ tree
.
├── cmd
│   └── appname
│       ├── cmd
│       │   └── root.go
│       └── main.go
└── pkg
    └── greeting
        └── greeting.go
```

2. 要求参数列表使用结构体保存

```go
type Person {
    Name string
    Age int
}
```

**注意**， 拆分目录结构之后， 就会出现 **包函数（跨文件夹）** 的调用， golang 是不允许 **循环依赖** 的。

## 扩展作业

什么是循环依赖？
