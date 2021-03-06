# C++Note  （知识点关键词）
## 基础知识
- if和switch的区别，效率性能
- C++基础知识， 常见关键词
> 提几个关键词：auto, decltype, nullptr，extern， static， const & volatile，operator， sizeof，this, template, typedef, typeid, typename, virtual,
> synchronized
- 预编译指令
>  pragma, if
elif
else
endif
ifdef
ifndef
define
undef
include
line
error
pragma
defined
 __has_include (since C++17)
 __has_cpp_attribute (since C++20)

- 散列表（哈希表）的原理，冲突问题，散列表如何解决冲突问题
- 内联函数，宏定义函数和普通函数的区别
- 指针与引用的区别
- new与malloc的区别
- 权限修饰符public，protect， private
- C++中类与结构体的区别？(默认访问权限不同)
- 列表初始化问题？
- 重载与重写的区别？
- 类型安全以及C++中的类型转换？
> static_cast, dynamic_cast, const_cast, reinpreter_cast的区别
- const与#define的区别
- 哪些函数不能成为虚函数？
- this指针的理解
- 构造函数 & 析构函数
- 拷贝构造函数，深拷贝，浅拷贝。  （注：移动构造函数问题，浅拷贝即可，因为对象赋值时是直接使用内存空间后删除原对象，拷贝构造函数参数是左值引用，而移动构造函数参数是右值&& 在STL中可以看到很多）
- 形参带&， && （左值引用，右值引用）
- 函数指针，回调函数
## 内存管理，内存泄漏
- 野指针
- 智能指针（引用计数）：auto_ptr，unique_ptr，share_ptr，weak_ptr
- 指针指向常量区
- 越界
## 各个版本的新特性 （C++11特性，C++14特性，C++17特性， C++20特性）
- C++11 ： nullptr, auto类型推导， labmda表达式.....
- C++14:
- C++17:
- C++20:
## STL --- 容器，迭代器，算法，仿函数
- vector（基于数组）内部进行多次拷贝容易造成内存碎片
- map
- list（基于双链表，每个节点保存上下节点指针）
- 函数对象
## 多态&继承
- C++内存模型
- 虚函数，纯虚函数
- 虚函数表，虚函数指针 （虚函数表初始化时期<函数时期：预编译，编译，汇编，链接>：：编译期）
- 抽象类（有纯虚函数的class），某基类中的函数全是纯虚函数，可看作java中的接口
- 虚继承
- 静多态&动多态 （编译时多态&运行时多态）： 模板属于静多态
- 动态绑定与静态绑定
## Linux
- poll，epoll，select区别
- 工具: GDB， VI\VIM
## 多线程
- 多线程同步 （互斥量，事件，临界区）
- 线程间通信（共享内存，信号，管道...） 其他：Socket，共享文件， 全局变量
## 网络socket编程
- socket流程
- 服务端： 创建socket，绑定端口（binding），监听，收发， 销毁
- 客户端： 创建socket，绑定， 收发数据， 销毁

## 设计模式
- 单例模式
> 懒汉式
> 饿汉式
- 工厂模式
- 适配器模式
- .......
## 模板
- 类模板，模板类，函数模板，模板函数
- 不定参数模板
- 模板的实例化： 隐式实例化、显式实例化
- 模板的特化： 全特化，偏特化（偏特化分两种：部分特化，对类型范围的限制，主要的模板类型基础不变），模板对模板进行特化。模板的特化是对模板的非通用部分进行特殊化处理。
- 模板类的继承
### C++函数或函数模板的匹配顺序

- 在有多个函数和函数模板名字相同的情况下，一条函数调用语句到底应该被匹配成对哪个函数或哪个模板的调用呢？ 
- C++ 编译器遵循以下先后顺序：
>  先找参数完全匹配的普通函数（非由模板实例化得到的函数）。
>  再找参数完全匹配的模板函数。
>  再找实参经过自动类型转换后能够匹配的普通函数。
>  如果上面的都找不到，则报错。
## stdarg.h 头文件

## CLR （C++， C#多语言环境）
- _declspec(dllexport)
>  C++导出函数
>  C++导出类
- _declspec(dllimport)

## 其他
- 实现printf（）格式化数据输出功能的思路
- 万用指针 void*

## 排序算法
- 常见算法  Pending......

## 分布式
- 分布式存储

## 其他开源工具库
- ONVIF 网络摄像头开源协议
- gSoap C++ webservice
- OSG(Open Scence Graphic)
- OpenGL
- OPenCV
- OCC （OPEN CASCADE）
- Epplus Excel处理库
- gmsh 三维有限元分割库 .STL文件
- Eigen 一个数学计算库
- fltk 轻量级图形界面库
- redis
- Wix3/Wix4 tool set 打包制作windows安装程序
