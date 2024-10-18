---
title: python回调函数
date: 2024-10-17
type: feature
tags:
  - python
---

# python回调函数

```py
# 定义回调函数
def my_callback(result):
    print(f"回调函数被调用，结果是: {result}")

# 定义一个接受回调函数的函数
def process_data(data, callback):
    # 处理数据
    result = sum(data)  # 简单处理：求和
    # 调用回调函数并传递结果
    callback(result)

# 使用示例
data = [1, 2, 3, 4, 5]
process_data(data, my_callback)
```


