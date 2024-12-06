# 项目简介
基于种子优化变异的网络协议模糊测试技术研究

# 工具简介
dragonafl 基于大模型智能生成高质量协议语法模板，驱动协议结构化智能变异。

# 灵感来源
chatafl: https://github.com/ChatAFLndss/ChatAFL

# 项目日志
- [x] 12/6，ddl快来了，开始做该项目
  
# 项目使用
## 安装依赖
```./deps.sh```

## 准备docker镜像
我们使用智谱的api

```KEY=<OPENAI_API_KEY> ./setup.sh```

## 运行
```./run.sh <container_number> <fuzzed_time> <subjects> <fuzzers>```
譬如说，这样的例子：
```./run.sh 1 5 pure-ftpd chatafl```

## 结果分析
```./analyze.sh <subjects> <fuzzed_time> ```