## Welcome to python-helping

You can use the [python-helping](https://zhuxilei.github.io/python-helping-txt/) to help you learn the Python.

你可以使用这个网站来帮助你学习Python。


### 1.注释 Comment
使用“#”来注释代码
use "#" to make a comment 
```markdown
a = 1
#将1赋值给a
```
### 2.输出 Output
print作为Python中最常用的一种输出方式将print后面的内容输出到屏幕。
print会将它后面的表达式当做字符串来输出并自动加入换行，当我们相接多个表达式时，只要在表达式间加上逗号就可以了。
```markdown
print "I am", 24, "years old"
```
### 3.元组
如果在定义list的时候将中括号变为小括号，我们就定义了Python中另一种数据结构，即元组。
```markdown
a = (1, 2, 3)
```
元组和list的主要区别在于元组内的元素是不可变的。

### 4.可以自定义索引的list -- dict
list这种以数字为索引的结构在面对一些日常生活中的问题会显得很麻烦，比如我们要设计一个通讯录，通讯录里存着人名和电话号码，我们希望通过名字来得到电话号码那么list就显得很不人性化了。
为此Python提供了另一种key-value存储形式的数据结构dict，我们可以定义自己的key来对整个dict进行索引。dict的形式也很简单，在大括号内用冒号分割key和value即可：
```markdown
contacts = {"LiLei" : "0101234", "HanMeimei" : "0101221365"}
print contacts["HanMeimei"]
```
由于dict不要求索引是连续的数字，这样我们的一些基本操作也和list不一样了，我们可以直接利用索引来进行插入、删除和更改操作，比如：
```markdown
contacts = {"LiLei" : "0101234", "HanMeimei" : "0101221365"}
```
#插入
```markdown
contacts["Lucy"] = "0108754696"
```
#更改
```markdown
contacts["LiLei"] = "0105689741"
```
#删除
```markdown
del contacts["HanMeimei"]
```

### 5.bool变量及运算
现实生活中我们经常会碰到一些关于是否的问题，比如"你学过Python么？"，"你喜欢我们的教程么？"，"1+1等于2么？"。
在Python中我们用True和False来回答这一类的问题，True和False就是所谓的bool值，注意他们的首字母都是大写哦。
在Python中有一系列的逻辑操作符号来帮助我们实现关于是否的判断，我们先来看一下最简单的相等判断，在Python中一个等号表示赋值，连续两个等号表示相等判断：
```markdown
print 1 + 1 == 2
```
既然有了相等判断自然也有不相等判断，用一个感叹号加上一个等号：
```markdown
print 1 + 1 != 2
```
除此之外Python还提供了在离散数学中常见的两个操作and和or。

and可以连接两个表达式，只要有一个表达式的结果为False整个表达式的结果即为False，只有当两个表达式结果都为True整个表达式的结果才为True。可以把and想象成一个严厉的判官，宁可错杀一千不可放过一个，一点错就把整个人否决掉。

or同样连接两个表达式，只要有一个表达式的结果为True整个表达式的结果即为True，只有当两个表达式结果都为False整个表达式的结果才为False。可以把or想象成一个仁慈的判官，只要还有一点是对的，那么就对整个人肯定。

它们的处理关系如下表所示：

expr1	 expr2	 expr1 and expr2	 expr1 or expr2
True	 True	        True	             True
True	 False	      False	             True
False	 True	        False	             True
False	 False	      False	             False

可以试下面的例子：
```markdown
print 1 + 1 == 2 and 1 + 1 == 3
print 1 + 1 == 2 or 1 + 1 == 3
```
除了上面两个性格不同的判官外，还有一个专门颠倒黑白的判官not他可以把True变成False把False变成True。
```markdown
print not 1 + 1 == 2
print not False
```
此外在编程中我们经常会碰到一类问题，即一个变量是不是在一个list或者dict中存在，最原始的想法就是拿这个list或dict中的每个变量和当前变量比较看看是不是相等，这么做写起代码来可就麻烦了，为此Python又用了一种优雅的方式解决了，既然你要解决一个变量在不在一组变量里这个问题，就新定义个操作就叫"在"吧，这就是我们的in操作：
```markdown
print 1 in [1, 2, 3]
print 4 not in [1, 2, 3]
```
### 6.
### 7.
### 8.
### 9.
网站部分资源来源于fenby.com
