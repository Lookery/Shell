# 数据结构
##   栈
##   数组
##  链表
当前节点 cur 值 val 下一个节点 next
节点 node
前节点 pre
##   哈尔表
表 dic 
# Python数据类型

切片操作
```
object[start_index:end_index:step]
```
step：正负数均可，其绝对值大小决定了切取数据时的‘‘步长”，而正负号决定了“切取方向”，正表示“从左往右”取值，负表示“从右往左”取值。当step省略时，默认为1，即从左往右以步长1取值。

start_index：表示起始索引（包含该索引对应值）；该参数省略时，表示从对象“端点”开始取值，至于是从“起点”还是从“终点”开始，则由step参数的正负决定，step为正从“起点”开始，为负从“终点”开始。

end_index：表示终止索引（不包含该索引对应值）；该参数省略时，表示一直取到数据“端点”，至于是到“起点”还是到“终点”，同样由step参数的正负决定，step为正时直到“终点”，为负时直到“起点”

## 数组(nums)
排序操作
```
nums.sort()
```
判断长度和维度
```
nums.size()
nume.shape()
```
## 列表(List)
判断长度和维度
```
len(list)
```
## 字典(Dic)
```
get(key[, value])
```
key -- 字典中要查找的键。
value -- 可选，如果指定键的值不存在时，返回该默认值。
查询是否在字典中有这个key
```
i in dic
```
## 字符串(Str)
Python和Java字符串都被设计成「不可变」的类型,因此修改需要赋给新的（C++可以）
```
list(s)
```
在输出时
```
return "".join(s)
```
可以查找修改字符串的命令
```
s.replace(" ","%20")
```

# collections模块
双向队列（deque）
类似于list的容器，可以快速的在队列头部和尾部添加、删除元素
```
append()
appendleft()
extend()
extendleft()
pop()
popleft()
count()
insert(index,obj)
rotate(n)
clear()
remove()
maxlen
```
计数器（Counter）
dict的子类，计算可hash的对象

默认字典（defaultdict）
dict的子类，可以调用提供默认值的函数

有序字典（OrderedDict）
dict的子类，可以记住元素的添加顺序

可命名元组（namedtuple）
可以创建包含名称的tuple
