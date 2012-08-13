Definitions 定义
================

由于该标准的用途，如下定义被使用。

Information object specification 信息对象说明
---------------------------------------------
这篇国际标准使用了定义在ITU-T Rec. X.681 | ISO/IEC 8824-2中的术语。
 * information object;(信息对象)
 * information object class;(信息对象类)
 * information object set;(信息对象集合)
 * instance-of type;(实例化类型)
 * object class field type.(对象类域类型)
 
Constraint specification 约束说明
---------------------------------
这篇国际标准中使用了定义在ITU-T Rec. X.682 | ISO/IEC 8824-3中的术语:
 * component relation constraint;(组件关联约束)
 * table constraint.(表约束)
 
Parameterization of ASN.1 specification ASN.1的的参数说明
---------------------------------------------------------
这篇国际标准中使用了定义在ITU-T Rec. X.683 | ISO/IEC 8824-4中的术语:
 * parameterized type;(参数化类型)
 * parameterized value.(参数化值)

Structure for identification of organizations 组织标识结构
----------------------------------------------------------
这篇国际标准中使用了定义在ISO/IEC 6523中的术语:
 * issuing organization;
 * organization code;
 * International Code Designator

Universal Multiple-Octet Coded Character Set (UCS) 通用多字节字符集
-------------------------------------------------------------------
这篇国际标准中使用了定义在ISO/IEC 10646-1中的术语:
 * Basic Multilingual Plane (BMP);
 * cell;
 * combining character;
 * graphic symbol;
 * group;
 * limited subset;
 * plane;
 * row;
 * selected subset.

附加的定义
----------

abstract character 抽象字符
^^^^^^^^^^^^^^^^^^^^^^^^^^^
抽象字符是用来组织，控制和表示文本数据的。

**NOTE**- :doc:`appendix/F` 提供了关于抽象字符的更完整的描述.

abstract value 抽象值
^^^^^^^^^^^^^^^^^^^^^
一个值，这个值的定义仅仅基于用于表达语义的类型，与它在任何编码中如何表达无关。

*NOTE*-抽象值的例子是整型,布尔型,字符串类型或者是整型、布尔型的序列(或候选)的值.

ASN.1 character set ASN.1字符集
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

[第十条]:todo:中描述的用在ASN.1符号中的字符的集合.

ASN.1 specification ASN.1说明
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
一个或多个ASN.1模块的集合。

associated type 关联类型
^^^^^^^^^^^^^^^^^^^^^^^^
关联类型是一个仅仅用于定义值或定义一种类型的子类型符号。

*NOTE*-关联类型在本标准中定义，仅仅是因为必须说明ASN.1中类型的定义与编码之间的显著差别。关联类型的定义并未出现在用户说明中。

bitstring type 位串类型
^^^^^^^^^^^^^^^^^^^^^^^
一个表示0至多个位序列的简单类型

*NOTE*-使用没有内容约束的bitstring(或者octetstring)类型的值来携带嵌入式的抽象值编码的方法已经废弃了.相反的使用embedded-pdv类型提供的机制更灵活,这种类型允许声明嵌入式抽象值的抽象语法和编码规则.

boolean type 布尔型
^^^^^^^^^^^^^^^^^^^
有两种不同值的简单类型

character property 字符属性
^^^^^^^^^^^^^^^^^^^^^^^^^^^
与定义字符指令表中的每一项相关联的信息集合。

*NOTE*-这些信息通常会包含下面的部分或全部项目:
 * 图形符号
 * 字符名
 * 与在特殊环境下使用的字符相关联的函数定义 
 * 是否代表一个数字
 * 在(大写/小写)情况下与之相关的不同的字符

character abstract syntax 字符抽象语法
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
任何使用一系列特定字符集而组成的特定字符串(0，1，或更多字符)而形成的语法

character repertoire 字符指令集
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
在字符集合中那些与编码独立的字符

character string types 字符串类型
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
一种使用某特定字符集中形成一串字符的简单类型。

character transfer syntax 字符传输语法
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
任何字符抽象语法的传输语法

*NOTE*-ASN.1不支持那些不把所有的字符串编码成为8位的整数倍的字符传输语法.

choice types 选择类型
^^^^^^^^^^^^^^^^^^^^^
通过引用一个不同的类型的列表来定义的类型;CHOICE类型的每一个值都来自于相应的组件类型的值.

component type 组件类型
^^^^^^^^^^^^^^^^^^^^^^^
当定义 **CHOICE**, **SET**, **SEQUENCE**, **SET OF** 或者 **SEQUENCE OF** 时引用的类型中的一种类型。 

constraint 约束
^^^^^^^^^^^^^^^
一个可以用来与一个类型相关联,来定义这个类型的子类型的符号。

contents constraint 内容约束
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
应用于bitstring或者octetstring上的约束, 这种约束要么是制定ASN.1类型的编码内容或者是用来出来内容的程序。

control  characters 控制字符
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
在一些字符条目中的字符,这些字符有名字(并且可能在某些环境下被赋予一些相关的功能)但是没有图形符号,并且不是空格字符。

*NOTE* - HORIZONTAL TABULATION (9) and LINE FEED (10) 是控制字符的例子,它们在打印环境中拥有格式化功能. DATA LINK ESCAPE (16)是另一个控制字符的例子,它在通信环境下被赋予了一些功能.

Coordinated  Universal  Time  (UTC) 世界调整时间
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
由国际时间管理局维护的时间尺度,它基于标准频率和时间信号的协调时间形式.

*NOTE* 1 – 这个定义的原始文件是ITU-R Rec. TF.460-5. ITU-R将世界调整时间的缩写定义为UTC.

*NOTE* 2 – UTC和格林威治时间(GMT)是可选的两个时间标准,大部分情况下确定的时间是相同的.

element 元素
^^^^^^^^^^^^

一个给定类型的值或者给定信息对象类的信息对象,与相同类型的全部其他值或者相同类的其他信息对象有所区别。

element set 元素集
^^^^^^^^^^^^^^^^^^

元素的集合,它们的所有元素都是给定类型的值或者给定类的信息对象。

*NOTE* – 给定类定义在ITU-T Rec. X.681 | ISO/IEC 8824-2

embedded-pdv type 嵌入的pdv类型
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
是一种类型,它的值的集合是几乎所有抽象语法的值的集合的组合.当想要传输协议的抽象值,这种值的类型采用ASN.1以外的描述定义的时候,embedded-dev类型可以用在ASN.1中来完成这样的描述.它携带了被传输的抽象值的抽象语法的标识符,作为编码这种抽象值的编码规范的标识符.

encoding 编码
^^^^^^^^^^^^^
将一套编码规则应用到一个抽象值之后得到的位模式的结果.

(ASN.1) encoding rules ASN.1编码规则
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
转换ASN.1类型的值的时候指定的一套规则.编码规范通过给定类型的知识,也允许从编码后的结果中恢复原来的值.

*NOTE* - 为了指定特别的编码规则，许多引用的类型(和值)的记号，其可以提供对于内建类型或值的可选记号，是不相关的。

enumerated types 枚举类型
^^^^^^^^^^^^^^^^^^^^^^^^^
一种简单类型,它的值是给定的标识符,这些标识符是类型定义符号的一部分。

extension addition 扩展添加
^^^^^^^^^^^^^^^^^^^^^^^^^^^
在扩展列表中添加的符号中的一个.对于SET, SEQUENCE和CHOICE类型,每一个扩展添加要么是单独的扩展添加组或者是单一一个组件类型.对于枚举类型,扩展添加都是将来要添加的枚举项.对于约束扩展添加是一个子类型元素.

*NOTE* – 扩展项是文本有序的(扩展符号后面)以及逻辑有序(具有增序枚举值,在CHOICE可选项中是增序标签)

extension addition group 扩展添加组
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
使用版本括号组合到一起的一个或者多个SET, SEQUENCE或CHOICE类型的一个或者多个组件.扩展添加组被用来清晰的标识SET, SEQUENCE或者CHOICE类型的组件,这些组件被添加在特定版本的ASN.1模块中,同时能够使用简单的整型表示版本.

