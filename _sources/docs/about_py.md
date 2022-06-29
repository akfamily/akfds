---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.12
    jupytext_version: 1.6.0
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(about_py)=

# 关于 AKFDS

> “AKFDS 是一个开源财经知识库项目，主要是为了方便查阅相关的财经知识而建立的，
> 所有人都可以向该库提交内容“ -- Albert King

## 什么是 AKFDS

AKFDS 是一个关于财经数据科学知识的开源知识库，作者是 [Albert King](https://www.akshare.xyz/)。

AKFDS 创建的主要目的是为了方便财经数据科学爱好者、数据科学家及相关人士查询相关的财经资料，
能够提高在财经数据科学领域的工作效率，也可以作为茶余饭后学习的园地。

作者还有其他开源项目，欢迎引用 {cite}`aktools2021`, {cite}`awesome-data2021` and {cite}`akshare2019`.

### 如何使用 AKFDS

AKFDS 的使用非常简单，您只需要访问项目主页：https://akfamily.github.io/akfds 就可以查看最新的知识库信息。

同时，AKFDS 还支持在线搜索您需要的资源，您只需要在搜索栏输入相关的关键词，就可以一键直达您需要的信息。

### 预览 AKFDS

The following chart, produced using Stack Overflow Trends, shows one
measure of the relative popularity of Python

```{figure} /_static/lecture_specific/about_py/python_vs_matlab.png
:scale: 72%
```

The figure indicates not only that Python is widely used but also that
adoption of Python has accelerated significantly since 2012.

This is driven at least in part by uptake in the scientific
domain, particularly in rapidly growing fields like data science.

For example, the popularity of [pandas](http://pandas.pydata.org/), a
library for data analysis with Python has exploded, as seen here.

(The corresponding time path for MATLAB is shown for comparison)

```{figure} /_static/lecture_specific/about_py/pandas_vs_matlab.png
:scale: 23%
```

Note that pandas takes off in 2012, which is the same year that we see
Python\'s popularity begin to spike in the first figure.

Overall, it\'s clear that

-   Python is [one of the most popular programming languages worldwide](http://spectrum.ieee.org/computing/software/the-2017-top-programming-languages).
-   Python is a major tool for scientific computing, accounting for a
    rapidly rising share of scientific work around the globe.

### ADFDS 的特点

Python is a [high-level language](https://en.wikipedia.org/wiki/High-level_programming_language)
suitable for rapid development.

It has a relatively small core language supported by many libraries.

Multiple programming styles are supported (procedural, object-oriented, functional, etc.)

Python is interpreted rather than compiled.

### Syntax and Design

One nice feature of Python is its elegant syntax --- we\'ll see many
examples later on.

Elegant code might sound superfluous but in fact it\'s highly beneficial
because it makes the syntax easy to read and easy to remember.

Remembering how to read from files, sort dictionaries and other such
routine tasks means that you don\'t need to break your flow in order to
hunt down correct syntax.

Closely related to elegant syntax is an elegant design.

Features like iterators, generators, decorators and list comprehensions
make Python highly expressive, allowing you to get more done with less
code.

[Namespaces](https://en.wikipedia.org/wiki/Namespace) improve
productivity by cutting down on bugs and syntax errors.

## 科学计算

Python has become one of the core languages of scientific computing.

It\'s either the dominant player or a major player in

-   [machine learning and data science](http://scikit-learn.org/stable/)
-   [astronomy](http://www.astropy.org/)
-   [artificial intelligence](https://wiki.python.org/moin/PythonForArtificialIntelligence)
-   [chemistry](http://chemlab.github.io/chemlab/)
-   [computational biology](http://biopython.org/wiki/Main_Page)
-   [meteorology](https://pypi.org/project/meteorology/)

Its popularity in economics is also beginning to rise.

## 参考文献

```{bibliography} ../_bibliography/references.bib
```
