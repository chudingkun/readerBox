### 从Borg到kubernates

为了解决管理全球数百万规模服务这个问题，谷歌开发一套私有的容器编排系统***[Borg](https://github.com/chudingkun/readerBox/blob/master/talk/ops/borg.md)***。Borg本质上是一个集中式的管理系统，它能将容器编排到服务池中。非常强大，borg同时也非常依赖google自己的核心技术，所以使得它非常难以被借鉴，以及更不可能开放出去。

直到2014年，google发现了一款名叫kubernates服务编排器，他建立在borg基础之上，并且还是开源的。当时市场上其实还有其他很多中服务编排器，但是都是商业收费的。直到2017年，kubernates开始大范围的使用了。

### kubernates的优势

一位叫Kelsey Hightower的谷歌高级开发，Kubernetes Up & Running的作者之一，kubernates社区的传奇人物。他说道：

> kubernates做的事情，最好的系统管理员也会这么去做：自动化、灾备、集中日志、告警，提供了很多开箱即用的功能。

很多的系统管理员疲于奔命的去升级系统、安装安全补丁、配置网络和各种备份。kubernates可以自动完成这些事情，这样你的团队就更放心的去做一些更重要的事情了。

kubernates的一些特性，比如负载均衡和自动伸缩，其他的包括可扩展的，第三方的工具都可以通过kubernates API 实现，kubernates的生态圈是很丰富的，而且一直在快速增长。

#### kubernates使开发更容易

运维人员喜欢kubernates有这些原因：kubernates很好的节省了运维的时间和精力，它提供了零停机，滚动更新等功能（当启动一个新容器的时候，直到新容器稳定启动完成，再关系旧的容器）

