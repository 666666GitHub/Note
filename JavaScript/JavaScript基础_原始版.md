# JavaScript基础

## day01

### 1.JS简介

JavaScript 是互联网上最流行的脚本语言，这门语言可用于 HTML 和 web，更可广泛用于服务器、PC、笔记本电脑、平板电脑和智能手机等设备。

运行在客户端的编程语言（浏览器）的编程语言，实现人机交互的效果。

+ 网页特效（监听用户的行为作出对应的反馈）
+ 表单验证（针对表单数据的合法性进行判断）
+ 数据交互(获取后台的数据，渲染到前端)
+ 服务端编程（node.js）

![image-20230622165426081](C:\Users\gjh\AppData\Roaming\Typora\typora-user-images\image-20230622165426081.png)

![image-20230623085859677](C:\Users\gjh\AppData\Roaming\Typora\typora-user-images\image-20230623085859677.png)

![](C:\Users\gjh\AppData\Roaming\Typora\typora-user-images\image-20230623085816995.png)

**书写位置**

+ 内部
  + 在\</body>上方,直接写在HTML文件里，用\<script>标签包住
+ 外部
  + 代码写在以.js结尾的文件中
+ 内联
  + 写在标签内部

**注释**

+ 单行注释
  + 符号：//  (快捷键Ctrl + /)
+ 块注释
  + 符号：/**/  （快捷键 shift + alt + a）

**结束符**：; (可写可不写)

**输入输出语法**

+ 输出

  + ~~~javascript
    document.write("HELLO WORLD")//跳过页面渲染先被执行
    prompt()//跳过页面渲染先被执行
    ~~~

+ 输入

  + ~~~javascript
    alert("")
    console.log("控制打印台")
    ~~~

**字面量**（literal）

+ 数字字面量
+ 字符字面量
+ 数组字面量
+ 对象字面量

### 2. 变量

变量是用于存储信息的"容器"。

[变量（菜鸟）](https://www.runoob.com/js/js-variables.html)

+ 变量的声明

  + ~~~javascript
    let age
    ~~~

+ 变量的赋值

  + ~~~javascript
    age = 18
    let age = 18
    ~~~

+ 更新变量

  + ~~~javascript
    let age =18 //不允许多次声明一个变量
    age = 19
    ~~~

+ 声明多个变量

  + ~~~javascript
    let age = 18 , uname = "张三"//建议分开声明
    ~~~

+ 交换变量



**变量的本质**

内存：存储数据的地方，相当于一个空间

变量的本质：是程序在内存中申请用来存放数据的小空间

变量的命名规则与规范

1. 规则：必须遵守，不遵守报错（类比是法律层面）
   1. 不能用关键字
   2. 只能用下划线，字母，数字，$组成，且不能是数字开头
   3. 字母严格区分大小写
2. 规范：建议，不遵守不会报错，但不符合业内通识（类比是道德层面）
   1. 起名要有意义
   2. 遵守小驼峰命名法

输入姓名的案例

变量的拓展

**let和var区别**

在老版本使用var，let是为了解决var的一些问题

**var声明**



### 3. 常量

### 4. 数据类型

### 5. 数据类型的转换

### 6. 算术运算符