JS目前共有 **8** 种数据类型。


### 7种基本类型
其中 7 种**基本类型**，除了null外都可使用`typeof`运算符进行检查：
1. undefined：已声明未赋值的变量初始值
2. boolean：布尔值
3. number：64位双精度浮点型
4. string：字符串
5. symbol：符号类型，唯一且不可修改
6. bigint：任意精度格式的整数
7. null：空对象

基本类型又叫值类型，值类型的值是始终不变的，比如定义了`var a = 1`，虽然变量`a`可以重新赋值，但是`1`这个值本身是不会变的。

除了**null**和**undefined**，其他 5 种基本类型都有对应的包装对象(将基本类型的单词首字母改为大写即为对应包装对象)。

 ### 1种引用类型
1 种**引用类型**：**Object**。

在JavaScript中，几乎所有的对象都是Object类型的实例，它们都会从Object.prototype继承属性和方法。

Function、Array、Date以及上面基本类型的包装对象，实际上都是由Object派生的，都属于Object类(用instanceof运算符检测结果为true，如 `Function instanceof Object` )。

---
#### 参考资料
[1] [语法和数据类型](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Grammar_and_types#%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E5%92%8C%E7%B1%BB%E5%9E%8B)
