# proj132-llc-mem-bandwidth-allocation
优化公有云环境下对不同虚拟机的LLC(last level cache)与MBW(memory bandwidth)的分配策略


### 项目描述与背景
公有云环境下，租户可以选择多种VM规格来租用资源，VM的规格主要是指CPU、内存、网络、存储，云厂商会提供租户之间的隔离能力，但由于不同的VM运行在同一个Host上共享LLC与MBW，仍然存在共享资源会被不同的租户争抢、甚至恶意攻击的情况。
因此需要对不同租户之间提供LLC与MBW的隔离分配策略，使减少租户之间的干扰，优化LLC与MBW敏感VM的性能。

### 功能描述

#### 基础功能：
1. 数据获取：选择合适的Metric数据，进行采集，并尽量保证较小的性能损耗。
2. 构建模型：聚合不同Metric，量化不同VM之间LLC/MBW的竞争情况，作为分配策略的输入。
3. 实现策略：根据竞争数据，实现分配策略，减少VM之间的LLC/MBW竞争，优化整体性能。


#### 扩展功能：


### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，参赛对象为全国普通高等学校全日制在校本科生和在校研究生，参赛队员的在校本科生或在校研究生身份均以报名时为准
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2022全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

周宜波 zhouyibo@bytedance.com

王楠 wangnan.light@bytedance.com




### 难度

中等


### 参考资料
[resctrl](https://www.kernel.org/doc/html/latest/x86/resctrl.html)

[intel-cmt-cat](https://github.com/intel/intel-cmt-cat/wiki)  



### License

* [GPL-2.0](https://opensource.org/licenses/GPL-2.0)



## 预期目标

完成基础的开发并输出说明文档一篇。

**注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标**

参考任务描述部分。
