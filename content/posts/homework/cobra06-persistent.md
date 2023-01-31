---
title: "Cobra06 - 持久化任务与参数"
subtitle: "Cobra05 Completion"
categories:
  - 半月刊
tags:
  - 半月刊202302A
  - 一般
date: "2023-01-16T22:47:01+08:00"
lastmod: "2023-01-16T22:47:01+08:00"
toc: true
draft: false
hiddenFromHomePage: false
pinTop: false
---



# Cobra07 - 命令行自动补全 （简单）

## 提示

```go

func main() {
	root := cobra.Command{
		PersistentPreRun:  func(cmd *cobra.Command, args []string) {},
		PersistentPostRun: func(cmd *cobra.Command, args []string) {},
	}

	root.PersistentFlags()
}
```

## 作业要求

在 cobra 中提供了 **Persistent** Run 和 Flag，

1. 作用是什么？
2. 父子孙命令之间， 是否具有继承关系？ 优先级是什么？

自己想一段功能实现。 并论证。
