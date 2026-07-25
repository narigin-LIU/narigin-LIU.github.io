---
title: "Hello World"
date: 2026-07-24
draft: false
categories: "test"
---

## 代码高亮

内置 Chroma 语法高亮，支持大多数编程语言：

```python
def binary_search(arr: list[int], target: int) -> int:
    """在有序数组中查找目标值的索引"""
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = left + (right - left) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
```

```rust
fn main() {
    let numbers: Vec<i32> = (1..=10).collect();
    let sum: i32 = numbers.iter().sum();
    println!("Sum of 1..10 = {sum}");
}
```

## LaTeX 数学公式

行内公式：$e^{i\pi} + 1 = 0$ （欧拉公式）。

块级公式：

$$
\frac{d}{dx} \int_a^x f(t)\,dt = f(x)
$$

矩阵：

$$
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

## 引用

> 代码是写给人看的，顺便能在机器上运行。
> — Structure and Interpretation of Computer Programs

## 表格

| 工具 | 用途 | 复杂度 |
|------|------|--------|
| Hugo | 静态站点生成 | 低 |
| KaTeX | 数学公式渲染 | 低 |
| Chroma | 代码语法高亮 | 零配置 |
