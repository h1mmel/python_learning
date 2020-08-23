### hello world!

---

python 环境部署成功后，就可以开始编写第一句python代码了。

新建 hello_world.py 文件，并使用ST打开，输入以下代码

```python
print('hello world!')
```

代码中的`print()`被称为`print函数` ，函数通常以`()`结尾，`()` 中包含的内容`'hello world!'`被称为是函数的参数。函数的参数可以为空也可以是一个或多个，具体要看函数是如何定义的，有关函数的内容会在之后具体学习。当python解释器运行脚本时，

使用`CTRL + S` 快捷键进行保存，也可以通过工具栏选择`File -> Save` 进行文件保存。

使用`F5` 快捷键运行此python脚本，运行成功后会在新标签页`*REPL* [python]`显示以下输出

```python
hello world!

***Repl Closed***
```

除了可以使用sublime text 3来运行python代码，python本身也自带了一个可以运行在终端窗口的解释器，这样就可以在终端窗口中输入python命令来打开python解释器。如下所示

```bash
Microsoft Windows [版本 10.0.18363.1016]
(c) 2019 Microsoft Corporation。保留所有权利。

C:\Users\xxxxx>python
Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> print('hello world!')
hello world!
>>>
```

同样的，也可以在终端直接运行python脚本文件，如下所示

```bash
Microsoft Windows [版本 10.0.18363.1016]
(c) 2019 Microsoft Corporation。保留所有权利。

C:\Users\xxxxx>python C:\Users\xxxxx\Documents\GitHub\python_learning\02-python基本语法\Code\hello_world.py
hello world!

```

至此，基本python环境已部署完毕，第一句python代码也已经成功运行，接下来就需要学习python的基础语法了。

