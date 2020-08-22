## 变量

###  变量命名

* 变量名只能包含字母、数字和下划线，且变量名不能以数字开头。
* 变量名不能包含空格。
* 不能使用python关键字和函数名用作变量名。

> 关键字表

| 1      | 2        | 3       | 4        | 5      |
| ------ | -------- | ------- | -------- | ------ |
| False  | class    | finally | is       | return |
| None   | continue | for     | lamda    | try    |
| True   | def      | from    | nonlocal | while  |
| and    | del      | global  | not      | with   |
| as     | elif     | if      | or       | yield  |
| assert | else     | import  | pass     |        |
| break  | except   | in      | raise    |        |

> 内置函数表 (python2.7)

| 1             | 2           | 3            | 4           | 5              |
| :------------ | ----------- | ------------ | ----------- | -------------- |
| abs()         | divmod()    | input()      | open()      | staticmethod() |
| all()         | enumerate() | int()        | ord()       | str()          |
| any()         | eval()      | isinstance() | pow()       | sum()          |
| basestring()  | execfile()  | issubclass() | print()     | super()        |
| bin()         | file()      | iter()       | property()  | tuple()        |
| bool()        | filter()    | len()        | range()     | type()         |
| bytearray()   | float()     | list()       | raw_input() | unichr()       |
| callable()    | format()    | locals()     | reduce()    | unicode()      |
| chr()         | frozenset() | long()       | reload()    | vars()         |
| classmethod() | getattr()   | map()        | repr()      | xrange()       |
| cmp()         | globals()   | max()        | reversed()  | zip()          |
| compile()     | hasattr()   | memoryview() | round()     | `__import__()` |
| complex()     | hash()      | min()        | set()       | ***apply()***  |
| delattr()     | help()      | next()       | setattr()   | ***buffer()*** |
| dict()        | hex()       | object()     | slice()     | ***coerce()*** |
| dir()         | id()        | oct()        | sorted()    | ***intern()*** |

注：python2.7中，print是关键字而不是函数。可以在脚本头部添加`from __future__ import print_function` 语句将print转换成函数使用。内置函数***apply()***、***buffer()***、***coerce()***、***intern()***被放进了[Non-essential Built-in Functions](https://docs.python.org/zh-cn/2.7/library/functions.html#non-essential-built-in-funcs) section中，不在重要。

> 内置函数表（python3.8）

| 1             | 2           | 3            | 4            | 5              |
| :------------ | ----------- | ------------ | ------------ | -------------- |
| abs()         | delattr()   | hash()       | memoryview() | set()          |
| all()         | dict()      | help()       | min()        | setattr()      |
| any()         | dir()       | hex()        | next()       | slice()        |
| ascii()       | divmod()    | id()         | object()     | sorted()       |
| bin()         | enumerate() | input()      | oct()        | staticmethod() |
| bool()        | eval()      | int()        | open()       | str()          |
| breakpoint()  | exec()      | isinstance() | ord()        | sum()          |
| bytearray()   | filter()    | issubclass() | pow()        | super()        |
| bytes()       | float()     | iter()       | print()      | tuple()        |
| callable()    | format()    | len()        | property()   | type()         |
| chr()         | frozenset() | list()       | range()      | vars()         |
| classmethod() | getattr()   | locals()     | repr()       | zip()          |
| compile()     | globals()   | map()        | reversed()   | `__import__()` |
| complex()     | hasattr()   | max()        | round()      |                |

注：python3.8中删除了内置函数basestring()、cmp()、execfile()、file()、long()、raw_input()、reduce()、reload()、unichr()、unicode()、xrange()，新增了内置函数ascii()、breakpoint()、bytes()、exec()。

</br>

### 字符串

* python 中以引号括起的都是字符串，引号可以是单引号('')和双引号("")

```python
'hello world!'
"hello world!"
```

如果字符串本身需要使用某种引号时，可以用如下方式解决

```python
"it's hers."
"I think 'python' is the best programming language."
'"python is the best."'
```

##### 字符串的常用方法

* 修改字符串的大小写

```python
name = 'guido van rossum'
print(name.title())
print(name.upper())
print(name.lower())
```

运行结果如下

```
Guido Van Rossum
GUIDO VAN ROSSUM
guido van rossum
```



