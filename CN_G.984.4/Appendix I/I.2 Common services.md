# Appendix I

# OMCI common mechanisms and services


## I.2 Common services

通用服务包含以下内容：

a)     start-up phase of ONT;                      ONT的启动阶段；

b)     on demand circuit pack provisioning;        按需 线路 包 供应/配置；

c)     on demand circuit pack de-provisioning;     按需 线路 包 解供应/解配置；

d)     plug-and-play circuit pack provisioning;    即插即用 线路 包 供应/配置；

e)     plug-and-play circuit pack de-provisioning; 即插即用 线路 包 解供应/解配置；

f)     software image download;                    镜像软件 下载； 

g)     software image changes;                     镜像软件运行；

所有 列表中的services/服务 是are 被解释的explained 通过 scenario diagrams（场景图，情节图 ） 的使用（by the use of）

（所有列表中的服务s在场景图/情节图的使用use 中被解释）


## I.2.1 ONT的启动阶段

ONT 的启动阶段， 来自（from）view 的 OMCI 指针（the OMCI point fo view）， 属于两个 cases 的其中一个：

a)      the ONT is new to the OLT； 或者

b)      the OLT 已经 “saw” 这个 ONT 在这个 PON

The details of start-up scenarios also vary for ONTs with different configuration options, e.g.:

启动 scenarios 的细节 也是 对 不同配置选项的 ONTs 有所不同， 比如：

a)      待用 cardholders 的 ONT 在 PON IF and NUI both；

b)      ONT with integrated interfaces at both PON IF and UNI;

c)      ONT with cardholders at PON IF and integrated interfaces at UNI; and

d)      ONT with integrated interfaces at PON IF and cardholders at UNI.

这里以下的scenarios 将仅显示 case a) and case b)， 从中可以推断出 case c) and d). 附加的 scenarios 可以被衍生 for the cases where ONT 包含 通用 设备 and/or 保护（protected）设备

**注意** - 推荐的解决方案是 that cardholder and 线路管理实体（MEs） 应该总是 modelled （模式化的）， 不论（regardless of）ONT 是否有 integrated interface。 然而， port mapping package provides another way 来 匹配 异构/多种类的端口 to 单一的 parent 设备。

Figure I.2.1-1 显示了在双方/两边 with Cardholders 的 “新” ONT 启动阶段。

Figure

Figure

The behaviour of ...

Note that if ...

In general, ...

[Figure]

[Figure]

[Figure]

## I.2.2 Circuit pack provisioning/de-provisioning










