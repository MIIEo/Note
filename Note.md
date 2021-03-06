[TOC]
* * *
February 19, 2018 12:50 PM

##gcc -Wall选项
选项-Wall开启编译器几乎所有常用的警告——**强烈建议使用该选项**。
编译器有很多其他警告选项，但-Wall是最常用的。默认情况下GCC不会产生任何警告信息。当编写C或C++程序时编译器警告非常有助于检测程序存在的问题。

##gcc -lm选项
如果有用到math.h库等非gcc默认调用的标准库，请使用-lm参数

##gcc -g选项
选项-g表示在生成的目标文件中带调试信息

##\#include"FILE.H"和\#include&lt;FILE.H&gt;
语句#include "FILE.h"与#include &lt;FILE.h&gt;有所不同：前者在搜索系统头文件目录之前将先在当前目录中搜索文件‘FILE.h’，后者只搜索系统头文件而不查看当前目录。

* * *
February 20, 2018 8:55 AM
##做算法题建议
**不要总是想着去优化，先把代码实现了再说，哪怕用最笨的方法。**
因为现代计算机计算能力已经很强了，哪怕你写的代码复杂度相当高，程序也不会运行太长时间.
* * *
February 22, 2018 11:34 AM
##算法题中输入、输出样例的作用
* 明确规定输入输出格式;
* 给出一组或者几组测试数据和预期运行结果，方便验证自己程序的正确与否;
* 样例有时会给出你仅仅根据问题描述拿不准的边界情况的处理方案.

##算法题做对几要素
* 正确接收规定格式的输入
* 正确地对输入数据进行处理
* 正确按规定格式输出结果

##算法题易错点
* 死循环
* 输入、输出格式错误

##算法模板：判断一个数是否为素数
``` cpp
#include <math.h>
#include <cstdio>

bool is_prime(int n){
	for(int i=2;i <= int(sqrt(n));i++)
		if(n%i==0)
    		return false;
	return true;
}
```

##算法题解题步骤
* **起名字：**给输入数据起名字，此时并不写代码，只是起名字，不去构思数据输入部分的代码
1.对字符型输入数据能按字符进行访问
2.对字符串型输入数据能分别按串、字符访问
3.对整型数据能按变量名访问
* **写算法：**构思算法以满足题目需要（重点）
* **敲代码**
1.写输入、输出部分的代码，此时不求空间开辟最小，只求正确处理输入、输出数据
2.写中间部分算法代码
* **调程序：**调试程序使得代码正确
* **优化**

##Ubuntu14.04耳机没有声音，状态：已解决
* 控制台键入`alsamixer`，寻找headphone选项，并通过shift+m开启
* 保存设置，控制台键入`sudo alsactl store`

* * *
February 23, 2018 9:50 AM
##sort(first,last,cmp)
排序范围是`[first,last)`,注意**前开后闭区间**
编写cmp的时候注意升降序

* * *
February 24, 2018 8:54 AM
##learngit.md,在当前目录下另一个文档中

* * *
March 1, 2018 10:48 PM
##学习的目标
* 对于一软件系统,用什么方法可以提高运算速度,提高系统性能
* 对于没有确定结果的问题(往往是机器学习中的问题),用什么方法构建的系统可以提高系统的性能,才是我们要关注的,我们要转换思路,之前对于确定的问题,我们关注速度,而现在,我们已经把重心从速度转移到性能上,因为目前的瓶颈是性能,而速度可以通过购买完成高速计算的芯片来弥补,而结果准确性的提高产生的影响在目前来讲是决定性的.

##emacs全选,复制,粘贴命令
* 全选:C-x h
* 复制:M-w
* 粘贴:C-y

##PAT题目特点
* 从数据结构角度出发去命制题目,规律性很强,题目的梯度也很合适

##结构体变量赋值
* 直接可以**通过变量名赋值**

##[急急急]PAT1052题目的对应代码有BUG,与键盘缓冲区有关,无法排解

##自动机转C++代码
题目:PAT1052

##swap(left,right)函数
头文件:iostream
功能:交换left和right内容
命名空间:std

##g++ 编译错误
```bash
error: ‘>>’ should be ‘> >’ within a nested template argument list
 priority_queue<double, vector<double>, greater<double>> q;
                                                      ^
```
解释:编译器无法确定的歧义出现,">>"为输入运算符
编译器:gcc4.8.4

##Ubuntu14.04浏览器firefox安装flash插件
* 下载相应的.tar.gz包,解压
* 在解压目录下存在一个usr目录,和libflashplayer.so库
* 在终端里跳转到解压目录,执行如下命令
```bash
sudo cp libflashplayer.so /usr/lib/firefox-addons/plugins
sudo cp -r usr/* /usr
```
* 然后重启firefox,`Bingo!!!`

##PAT乙级1074题目出错


##mpich2安装
* tar -xzf mpich2-1.4.tar.gz
* cd mpich2-1.4
* ./configure
* make; sudo make install
* mpiexec --version


















