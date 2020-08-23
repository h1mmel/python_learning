## 变量

###  变量命名

* 变量名只能包含字母、数字和下划线，且变量名不能以数字开头。
* 变量名不能包含空格。
* 不能使用python关键字和函数名用作变量名。

> 关键字表（python2.7）

| 1        | 2       | 3      | 4      | 5     |
| -------- | ------- | ------ | ------ | ----- |
| and      | del     | from   | not    | while |
| as       | elif    | global | or     | with  |
| assert   | else    | if     | pass   | yield |
| break    | except  | import | print  |       |
| class    | exec    | in     | raise  |       |
| continue | finally | is     | return |       |
| def      | for     | lamda  | try    |       |

> 关键字表（python3.8）

| 1      | 2        | 3       | 4        | 5      |
| ------ | -------- | ------- | -------- | ------ |
| False  | await    | else    | import   | pass   |
| None   | break    | except  | in       | raise  |
| True   | class    | finally | is       | return |
| and    | continue | for     | lambda   | try    |
| as     | def      | from    | nonlocal | while  |
| assert | del      | global  | not      | with   |
| async  | elif     | if      | or       | yield  |

注：从python3.7开始新增了关键字，False、None、True、async、await、nonlocal，删除了关键字exec、print。关键字的使用必须表格中列出的拼写完全一致。

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

注：python2.7中，print是关键字而不是函数。可以在脚本头部添加`from __future__ import print_function` 语句将print转换成函数使用。内置函数***apply()***、***buffer()***、***coerce()***、***intern()*** 被放进了[Non-essential Built-in Functions](https://docs.python.org/zh-cn/2.7/library/functions.html#non-essential-built-in-funcs) section中。

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

#### 基本变量类型

---

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

##### 字符串的几种常用方法

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

> python变量使用句点(.)访问方法，如name.title()，代表变量name执行title()方法，作用就是将字符串中的每个单词的首字母大写。然后print()函数将name.title()的返回结果打印在终端上。同理，upper()方法作用是将字符串中的所有字符转换成大写，lower()方法作用是将字符串中的所有字符转换成小写，因为name本身就是小写所以没有变化。

注：python中的函数分为**函数**和**方法**两种叫法，其中类中的函数被称为方法。

* 拼接字符串

```
start = 'hello'
end = 'world!'
print(start + end)
```

