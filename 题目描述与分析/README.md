# 题目描述与分析

**项目描述**

Flash介质因本身的擦除特性，给上层文件系统带来与普通磁盘、内存文件系统不同的数据管理模式。同时，Flash的写入放大、寿命以及后期稳定性下降等问题也给文件系统的设计带来的一定的挑战。传统的Flash文件系统并没有很好地解决这些稳定性相关问题。这里希望寻找一种更智能、更合适的Flash文件系统设计，来更好地平衡Flash的性能与稳定性。可以思考的方向包括但不限于：数据压缩算法（可以是自适应的压缩算法），检错、纠错、纠删码（可以是联合信源信道编码），数据块选择、擦除策略，Cache机制。

**项目导师**

* 郑立铭
* email: [zhengliming3@huawei.com](mailto:zhengliming3@huawei.com)

**难度**

中等

**特征**

* 完成基本的文件系统的功能。
* 合理地使用数据压缩方案，平衡计算性能与Flash写入性能。
* 设计擦除块选择算法、数据块迁移算法，平衡各擦除块寿命、减少写入放大。

**进阶特性**

* 设计写入Cache，提升写入速率，同时需要考虑数据的一致性与可持久化(可以说是掉电)问题，可以结合类似Trim的机制。
* 设计一个自适应的Flash纠错编码。识别Flash的生命周期，在Flash的生命周期前期倾向性能，后期倾向稳定性。

**概括：**要求设计一个更智能的 Flash 文件系统，包括以下特性：

* 完成基本的文件系统的功能。
* 合理地使用数据压缩方案，平衡计算性能与 Flash 写入性能。
* 设计擦除块选择算法、数据块迁移算法，平衡各擦除块寿命、减少写入放大。
* 设计写入 Cache，提升写入速率，同时需要考虑数据的一致性与可持久化问题，可以结合类似 Trim 的机制。
* 设计一个自适应的 Flash 纠错编码。识别 Flash 的生命周期，在 Flash 的生命周期前期倾向性能，后期倾向稳定性。
