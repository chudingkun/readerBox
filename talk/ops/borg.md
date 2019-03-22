## 

 *译者原文：http://dockone.io/article/726 译者：难易   英文原文：https://github.com/chudingkun/readerBox/blob/master/books/ops/borg.pdf*

## 摘要 

谷歌的Borg系统群集管理器运行几十万个以上的jobs，来自几千个不同的应用，跨多个集群，每个集群有上万个机器。

它通过管理控制、高效的任务包装、超售、和进程级别性能隔离实现了高利用率。它支持高可用性应用程序与运行时功能，最大限度地减少故障恢复时间，减少相关故障概率的调度策略。Borg简化了用户生活，通过提供一个声明性的工作规范语言，名称服务集成，实时作业监控，和分析和模拟系统行为的工具。

我们将会展现Borg系统架构和特点，重要的设计决策，定量分析它的一些策略，和十年以来的运维经验和学到的东西。

<img src="https://raw.githubusercontent.com/chudingkun/readerBox/master/conf/picture/borg.jpg" title="wechat" width="200" /> 