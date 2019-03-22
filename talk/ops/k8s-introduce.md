### 从Borg到kubernates

为了解决管理全球数百万规模服务这个问题，谷歌开发一套私有的容器编排系统***[Borg](https://github.com/chudingkun/readerBox/blob/master/talk/ops/borg.md)***。Borg本质上是一个集中式的管理系统，它能将容器编排到服务池中。非常强大，borg同时也非常依赖google自己的核心技术，所以使得它非常难以被借鉴，以及更不可能开放出去。

直到2014年，google发现了一款名叫kubernates服务编排器，他建立在borg基础之上，并且还是开源的。当时市场上其实还有其他很多中服务编排器，但是都是商业收费的。直到2017年，kubernates开始大范围的使用了。

