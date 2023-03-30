# -
数据结构第一次作业vector
## vector.h
vector.h 包含了定义的成员函数并实现了成员函数
没有对complex重载操作符,给vector的find函数，search函数，bubblesort函数，mergesort函数 添加了 函数作为新参数 的参数，参数具体实现在main.cpp 中

考虑了少部分 函数的鲁棒性，例如插入元素时考虑秩是否合理 

## comlex.h 
在homewok文件夹中，定义了基本的成员参数和 随机化函数，求模函数

##main.cpp
### 第一部分 
 1.置乱
 2.插入
 3.删除
 4.查找   修改了 vector.h 的内容，使其更具有普遍性
 5.唯一化 修改了 vector.h 的内容，使其更具有普遍性
### 第二部分
 首先测试两个函数有用 ：bubblesort 和 mergesort
 其次乱序，正序，逆序比较各自运行时间               数据量在7000 （设置大了编译器老是出现奇奇怪怪的错误）
### 第三部分 
定义了 partqurry 和 mysearch 两个函数
mysearch 函数 效果：（升序时） 1.查的到时：找到不大于该元素的最小位置  2.查不到时： 找到大于这个数的最小位置  因此要对二分查找（C版本）做修改，不具有普遍性，故不写入 vector.h 文件中
partqurry 函数 ： 调用两次 mysearch 函数，找到子序列的秩，用构造函数返回子序列 
