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
 