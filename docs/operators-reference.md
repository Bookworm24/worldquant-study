# WorldQuant 操作符参考

## 数学运算符

### 基本运算符
- `+` : 加法
- `-` : 减法
- `*` : 乘法
- `/` : 除法 (注意: 当分母为0或无穷大时返回0)
- `^` : 幂运算

### 高级数学函数
- `pow(x, y)` : x的y次幂
- `sqrt(x)` : 平方根
- `log(x)` : 自然对数
- `exp(x)` : e的x次幂
- `abs(x)` : 绝对值
- `max(x, y)` : 返回较大值
- `min(x, y)` : 返回较小值
- `sign(x)` : 符号函数

## 条件运算符

### 逻辑运算符
- `and` : 逻辑与
- `or` : 逻辑或
- `not` : 逻辑非

### 比较运算符
- `==` : 等于
- `!=` : 不等于
- `>` : 大于
- `<` : 小于
- `>=` : 大于等于
- `<=` : 小于等于

### 条件函数
- `if(condition, true_value, false_value)` : 条件函数
- `gt_nansafe(x, y)` : 安全的大于比较（处理NaN值）

## 时间序列函数

### 延迟函数
- `delay(x, d)` : 将序列x延迟d个时期
- `delta(x, d)` : x - delay(x, d)，d期差分

### 排序和排名函数
- `ts_rank(x, d)` : d期内x的时序排名
- `ts_argmax(x, d)` : d期内x的最大值位置
- `ts_argmin(x, d)` : d期内x的最小值位置

### 统计函数
- `sum(x, d)` : d期内x的和
- `stddev(x, d)` : d期内x的标准差
- `correlation(x, y, d)` : x和y在d期内的相关性
- `covariance(x, y, d)` : x和y在d期内的协方差
- `sma(x, d)` : d期简单移动平均
- `wma(x, w, d)` : d期加权移动平均

## 横截面函数

### 排名和缩放
- `rank(x)` : 横截面排名
- `scale(x)` : 将x缩放到[-1, 1]
- `industry_neutral(x)` : 行业中性化

### 统计函数
- `group_neutral(x, g)` : 按组g对x进行中性化
- `ind_avg(x)` : 行业平均
- `ind_median(x)` : 行业中位数
- `ind_max(x)` : 行业最大值
- `ind_min(x)` : 行业最小值

## 常用数据字段

### 价格相关
- `PX_LAST` : 最后价格
- `PX_OPEN` : 开盘价
- `PX_HIGH` : 最高价
- `PX_LOW` : 最低价

### 基本面相关
- `MCAP` : 市值
- `PE_RATIO` : 市盈率
- `PB_RATIO` : 市净率
- `DIVIDEND_YIELD` : 股息率

### 交易量相关
- `VOLUME` : 成交量
- `VOLUME_AVG_30D` : 30日平均成交量

## 示例 Alpha 表达式

### 简单示例
```
rank(PX_LAST / delay(PX_LAST, 5) - 1)  # 5日收益率排名
```

### 复杂示例
```
rank(correlation(PX_LAST, volume, 10)) * rank(-ts_rank(PX_LAST, 10))  # 结合相关性和价格排名
```

## 学习建议

1. 从基本数学运算符开始
2. 理解时间序列函数的概念
3. 学习横截面函数的用途
4. 尝试组合不同类型的函数
5. 通过实际测试验证理解