# cloud_python
### python学习项目

Python 是一种解释型语言
在程序开发阶段可以为你节省大量时间，因为不需要编译和链接
Python 允许你将程序划分为能在其他的 Python 程序中重复利用的模块。它内置了很多的标准模块，你可以在此基础上开发程序——也可以作为例子

编码 encoding: utf-8 
# -*- coding: encoding -*-

python中的注释以井号 # 开头

>>> ---等待输入

>>> tax = 12.5 / 100
>>> price = 100.50
>>> price * tax
12.5625
>>> price + _
113.0625
>>> round(_\n 2)
113.06
> 在交互模式下，上一次打印出来的表达式被赋值给变量 _

数字类型 int 和 float，Python也支持其他类型的数字，例如 Decimal 或者 Fraction

字符串
Python 也可以操作字符串。字符串有多种形式，可以使用单引号（'...'），双引号（"..."）都可以获得同样的结果 
       反斜杠 \ 可以用来转义
       如果不希望前置了 \ 的字符转义成特殊字符，可以使用 原始字符串 方式，在引号前添加 r 即可
       字符串字面值可以跨行连续输入。一种方式是用三重引号："""...""" 或 '''...'''。字符串中的回车换行会自动包含到字符串中，如果不想包含，在行尾添加一个 \ 即可
        print("""\
        Usage: thingy [OPTIONS]
            -h                        Display this usage message
            -H hostname               Hostname to connect to
        """)
        字符串可以用 + 进行连接（粘到一起），也可以用 * 进行重复
        相邻的两个或多个 字符串字面值 （引号引起来的字符）将会自动连接到一起
        >>> 'Py' 'thon'
            'Python'
        字符串是可以被 索引 （下标访问）的，第一个字符索引是 0。单个字符并没有特殊的类型，只是一个长度为一的字符串
        除了索引，字符串还支持 切片。索引可以得到单个字符，而 切片 可以获取子字符串
        >>> word = 'Python'
        >>> word[0]  # character in position 0
        'P'
        >>> word[5]  # character in position 5
        'n'
        注意 -0 和 0 是一样的，所以负数索引从 -1 开始 ||| 右边开始数
        >>> word[0:2]  # characters from position 0 (included) to 2 (excluded)
        'Py'
        >>> word[2:5]  # characters from position 2 (included) to 5 (excluded)
        'tho'
        注意切片的开始总是被包括在结果中，而结束不被包括。这使得 s[:i] + s[i:] 总是等于 s

列表
Python 中可以通过组合一些值得到多种 复合 数据类型。其中最常用的 列表 ，可以通过方括号括起、逗号分隔的一组值（元素）得到。一个 列表 可以包含不同类型的元素，但通常使用时各个元素类型相同: