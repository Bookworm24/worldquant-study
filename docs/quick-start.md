# WorldQuant 学习系统快速入门

## 欢迎使用 WorldQuant 学习系统

这个学习系统是基于成功的 CFP 学习方法论设计的，专门为 WorldQuant 因子挖掘学习而定制。它使用 iFlow AI 作为您的个人导师，采用苏格拉底式教学方法来帮助您深入理解量化金融概念。

## 第一步：理解系统结构

### 目录结构
```
worldquant-study/
├── README.md                    # 项目概述
├── iFlow.md                     # iFlow AI 指令
├── sessions/                    # 学习会话记录
│   ├── 2025-12-25/            # 按日期组织的会话
│   │   └── session-notes.md    # 会话笔记示例
│   └── SESSION-TEMPLATE.md     # 会话记录模板
├── progress/                    # 进度跟踪
│   └── worldquant-study-tracker.md # 综合进度跟踪器
├── data/                        # WorldQuant 资料
│   ├── datasets-info/          # 数据集信息
│   ├── operators-info/         # 操作符信息
│   └── example-alphas/         # 示例因子
└── docs/                        # 学习文档
    ├── worldquant-platform-overview.md # 平台概述
    ├── operators-reference.md   # 操作符参考
    ├── iflow-learning-guide.md  # iFlow 学习指南
    └── evaluation-metrics.md    # 评估指标详解
```

## 第二步：开始学习

### 1. 设置您的学习环境
1. Fork 此仓库到您的 GitHub 账户
2. 克隆仓库到本地
3. 阅读 [iFlow.md](../iFlow.md) 文件以了解 AI 导师如何工作

### 2. 开始第一个学习会话
1. 在 [worldquant-study-tracker.md](../progress/worldquant-study-tracker.md) 中更新您的学习目标
2. 与 iFlow AI 开始对话，询问您感兴趣的主题
3. 记录学习过程和理解程度

### 3. 记录学习会话
1. 在 `sessions/YYYY-MM-DD/` 目录下创建新的会话笔记
2. 使用 [SESSION-TEMPLATE.md](../sessions/SESSION-TEMPLATE.md) 作为参考
3. 记录：
   - 学习的主题
   - 问过的所有问题
   - 您的初始理解
   - 概念解释
   - 理解检查结果
   - 发现的知识缺口
   - 掌握的主题

## 第三步：跟踪您的进度

### 更新进度跟踪器
定期更新 [worldquant-study-tracker.md](../progress/worldquant-study-tracker.md)：
- 标记已掌握的主题
- 记录发现的知识缺口
- 调整学习计划
- 更新学习统计数据

### 使用学习资源
- 阅读 [docs/](./) 目录下的文档
- 参考 [operators-reference.md](./operators-reference.md) 了解 WorldQuant 操作符
- 学习 [evaluation-metrics.md](./evaluation-metrics.md) 理解因子评估

## 第四步：与 iFlow AI 互动

### 有效的提问方式
- "iFlow，我想学习 WorldQuant 的基本概念"
- "请解释一下什么是信息系数 (IC)"
- "如何构建一个简单的价值因子？"
- "请给我一个使用 rank() 函数的例子"

### 验证理解
- 用自己的话解释概念
- 尝试构建简单的例子
- 询问相关概念之间的区别

## 学习建议

### 每日学习
- 每天至少学习 30 分钟
- 记录每次学习的要点
- 定期回顾之前学习的内容

### 每周评估
- 检查进度跟踪器
- 识别需要加强的领域
- 调整下周的学习计划

### 实践应用
- 尝试构建简单的因子
- 使用 WorldQuant 平台测试概念
- 将理论与实践相结合

## 进阶学习

### 初级阶段
- 理解基本的 WorldQuant 概念
- 学习常用操作符
- 构建简单的因子

### 中级阶段
- 学习时间序列和横截面函数
- 优化因子性能
- 理解评估指标

### 高级阶段
- 构建多因子模型
- 学习风险管理技巧
- 探索机器学习在因子挖掘中的应用

## 资源链接

- [WorldQuant 官方文档](https://www.worldquant.com/)
- [iFlow AI 学习指南](./iflow-learning-guide.md)
- [平台概述](./worldquant-platform-overview.md)
- [操作符参考](./operators-reference.md)
- [评估指标详解](./evaluation-metrics.md)

现在您已经了解了如何使用这个学习系统，开始您的 WorldQuant 学习之旅吧！