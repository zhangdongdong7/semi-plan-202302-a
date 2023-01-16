---
title: "cobra04 - 项目工程目录结构"
subtitle: "Cobra Layout"
categories:
  - 半月刊
tags:
  - 半月刊202302上
  - 简单
date: "2023-01-16T22:34:14+08:00"
lastmod: "2023-01-16T22:34:14+08:00"
toc: true
draft: false
hiddenFromHomePage: false
pinTop: true
---



# Cobra04 - 项目工程目录结构

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

