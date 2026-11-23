# 项目选择以及个人理解
#### 项目的仓库链接：https://github.com/langchain-ai/langchain.git
在了解了AI Agent运行工作的底层原理后，我尝试去了解一些与AI有关的项目，最终选择了langChain开源框架。
在AI助手的帮助下，我尝试阅读了该项目的README文件，下面用我的理解来介绍该项目的主要内容。
## 主要内容：
#### 根据核心公式agent=LLM+Harness，大模型本身只能聊天，不过加上了Harness，大模型就能调动外部工具，变成一个能干活的智能助手。那么langChain就是提供一个极简的、高度可配置的Harness框架，可以根据具体的使用场景以及数据来配置。
## 难道市场上就这一种Harness框架吗？
不是的。还有如OpenAI Agent SDK,Google ADK等等。
## 那为什么选择langChain呢（langChain的好处）？
- 标准模型接口：不同的大模型其擅长的领域也不同，langChain的标准模型接口可以帮助开发者切换不同的大模型，以便找到最适合任务开发使用的大模型
- 高度可配置的Harness框架：langChain中的creat_agent官方定义为最小的但高度可配置的Harness，开发者只需要往里面放所需的LLM，System prompt，tool，中间件等就行。
- 基于langGraph构建，使用langSmith调试：langChain在搭框架时，如果任务不是一问一答，而是需要反复思考甚至人工介入判断时，langChain就不够用了，需要langGraph来画流程图；AI跑起来后是个“黑盒”，有了langSmith我们就能监控AI内部每一步干了什么，调用了哪些工具，用来找bug和优化性能。
## langChain适合处理哪些问题？
langChain适合处理那些需要模型去接触调用外部数据和工具，反复思考，动手做事的问题。
- 查私有的数据（笔记、产品手册）
- 需要动手（查天气、算数据······）
- 多步骤任务（查阅资料写报告）
- 记住长对话内容（客服聊天）
- ······
## 感兴趣的原因
因为最近接触智能体底层原理比较多，所以项目选择的方向还是往AI上面去靠，并且在学习过程中，我对Harness的作用理解的并不是太深刻，也更想了解一下Agent反复思考的过程中，其内部的工具，任务规划等等是怎么协调配合的。
## 未来可以怎么实践
目前阶段我可以试着把我的学习笔记交给Harness的记忆模块，以后我问问题的时候，就可以及时找到对应的内容。

在将来，或许我可以试着在C语言的语法基础上去了解python的基本语法，再对Agent的搭建过程进行深入学习，尝试搭建一个自己的Agent。
# 开发和学习环境的搭建
我在github开源社区搜索浏览了langChain仓库，长远的想法有想要开发搭建一个属于自己的Agent。

编程语言：python（AI领域的语言python优先）

代码编辑器：VS Code（配置python插件）

AI助手: 选择Trae与GitHub Copilot


