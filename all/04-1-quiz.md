#lec8 在线练习
## 选择题

---
 
操作系统中可采用的内存管理方式包括() s1

- [x] 重定位(relocation)
- [x] 分段(segmentation
- [x] 分页(paging)
- [x] 段页式（segmentation+paging）

> 都有

在启动页机制的情况下，在CPU运行的用户进程访问的地址空间是() s2

- [ ] 物理地址空间
- [x] 逻辑地址空间
- [ ] 外设地址空间
- [ ] 都不是

>  用户进程访问的内存地址是虚拟地址

连续内存分配的算法中，会产生外碎片的是() s3

- [x] 最先匹配算法
- [x] 最差匹配算法
- [x] 最佳匹配算法
- [ ] 都不会

> 三种算法都会有外碎片

在使能分页机制的情况下，更合适的外碎片整理方法是() s4

- [ ] 紧凑(compaction)
- [ ] 分区对换(Swapping in/out)
- [x] 都不是

> 分页方式不会有外碎片

描述伙伴系统(Buddy System)特征正确的是() s5

- [x] 多个小空闲空间可合并为大的空闲空间
- [x] 会产生外碎片
- [x] 会产生内碎片
- [ ] 都不对

> 前三个是对的。

-----
