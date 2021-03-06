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

# 股票

本章主要给大家介绍什么是期货，期货的定义最早起源于美国，主要是在大宗商品
市场的买卖上

## 股票的定义

期货的定义：期货是在交易所交易的

## 股票交易市场

### 中国大陆

| 交易所名称                                 | 交易所代码 | 合约后缀  | 首页地址                     |
|---------------------------------------|-------|-------|--------------------------|
| [中国金融期货交易所](http://www.cffex.com.cn/) | CFFEX | .CFX  | http://www.cffex.com.cn/ |
| [上海期货交易所](http://www.shfe.com.cn/)    | SHFE  | .SHF  | http://www.shfe.com.cn/  |
| [上海国际能源交易中心](http://www.ine.cn/)      | INE   | .INE  | http://www.ine.cn/       |
| [郑州商品交易所](http://www.czce.com.cn/)    | CZCE  | .ZCE  | http://www.czce.com.cn/  |
| [大连商品交易所](http://www.dce.com.cn/)     | DCE   | .DCE  | http://www.dce.com.cn/   |
| [广州期货交易所](http://www.gfex.com.cn/)    | GFEX  | .GFEX | http://www.gfex.com.cn/  |

### 中国香港

| 交易所名称                                 | 交易所代码 | 合约后缀  | 首页地址                     |
|---------------------------------------|-------|-------|--------------------------|
| [中国金融期货交易所](http://www.cffex.com.cn/) | CFFEX | .CFX  | http://www.cffex.com.cn/ |
| [上海期货交易所](http://www.shfe.com.cn/)    | SHFE  | .SHF  | http://www.shfe.com.cn/  |
| [上海国际能源交易中心](http://www.ine.cn/)      | INE   | .INE  | http://www.ine.cn/       |
| [郑州商品交易所](http://www.czce.com.cn/)    | CZCE  | .ZCE  | http://www.czce.com.cn/  |
| [大连商品交易所](http://www.dce.com.cn/)     | DCE   | .DCE  | http://www.dce.com.cn/   |
| [广州期货交易所](http://www.gfex.com.cn/)    | GFEX  | .GFEX | http://www.gfex.com.cn/  |

### 中国台湾

## 股票的复权

### 什么是股票复权

复权，按字面意思理解，就是修复股权。不复权，就是不修复股权，不把除权的因素考虑进去，看到的是股价的实际价格。

一家企业在上市的时候，股本是确定的，发行总价也是确定的。比如说上市公司A上市时发行了100万元的股权，合计10000股，那么每股价格就是100元（以下都以此为例）。

如果公司后面几年从来没有发生过分红送股这些行为，那么在任意一个时间点，不复权价、前复权价和后复权价都是一样的。

问题就出现在发生了分红送股以后。分红，表示的是发放股利，也就是将上一年公司创造的利润的一部分发给股东；送股，其实也是另一种奖励，你本来持有100股，公司每10股送10股，那你就有200股了。

> 除权（exit right，XR）指的是股票的发行公司依一定比例分配股票给股东，作为股票股利，此时增加公司的总股数。例如：配股比率为25/1000，表示原持有1000股的股东，在除权后，股东持有股数会增加为1025股。此时，公司总股数则膨胀了2.5%。
> 除了股票股利之外，发行公司也可分配“现金股利”给股东，此时则称为除息。（红利分为股票红利与现金红利，分配股票红利对应除权，分配现金红利对应除息。）

分红送股以后，要保证这个操作不改变上市公司的总市值，也就是说保证（总股本数*每股价格）不变，那么就要进行除权除息。

到这里，可能有点蒙了。事实就是，分红送股虽然听上去是发放了红利，但这项操作最终折算下来并没有改变你手里的资产数目（牢记这一条，类似能量守恒定律）。

### 为什么要进行股票复权

股票回测的时候，如果回测的时间区间比较长，且中间存在分红、送股、拆分、合并等事件导致账户股票数目(或者权益)变化，
价格可能大幅度变化的情况下，就需要考虑是否对股票价格进行复权处理。

### 股票复权的种类

#### 不复权

还是以此为例，比如公司A要进行分红送股（10转8派50元），那么就是说，如果你持有A公司10股的股票，那么在发布分红公告后你的账户里将会额外得到8股的股票和5元的现金分红。

但我们要遵守“能量守恒定律”，分红送股并不改变原有的“能量”，那么分红送股后的股价变为多少了呢？

计算公式则为：

（100-5）/（1+0.8）=52.78

可以看到，分红送股前后股价出现了突变。

如果展示在K线图上，那就是一个阶跃性的变化，看上去就跟“腰斩”了一样。

不复权价表示的就是这个价格。

#### 前复权

#### 后复权

#### 定点复权

### 推荐的方式

