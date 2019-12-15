# java-web
### 程序开发体系
* C/S体系结构
>客户端和服务器结构，类比如在手机上王者荣耀——客户端，上传处理数据，发送到腾讯的服务器——服务器。
安全性好，升级复杂，不仅服务器端要升级，客户端也要升级。要对不同的机型开发不同的软件。
* B/S体系结构
>不需要安装软件，通过网页与服务器交互，安全性差，但是应用升级更改方便，不存在客户端也要升级的情况。

### 什么是web？
网页
分为静态和动态

### web前端
* html
通过标签元素描述网页的**内容**结构
* CSS
描述网页的**排版布局**
* javaScript（js）
描述网页的**事件处理**
**与jsp不同，jsp处理后端，js处理前端**

### 前端详解
#### html（超文本标记语言）
1. 是普通文本文件
2. 包含成对标签
3. 以htm或者html为扩展名
4. 可以在大多数浏览器上显示
##### 标签元素
```html
<html>
    <head>

    </head>
    <body>
        <h1>这里是标题</h1>
        <h6>我也是标题</h6>
        <p>这是一个段落</p>
        <a href="https://www.baidu.com/">
            在这个标签里添加链接</a>
        <!--这是一个注释-->
        <ul>
            <li>这是无序列表的第一行</li>
            <li>这是无序列表的第二行</li>
            <li>这是无序列表的第三行</li>
        </ul>
        <ol>
            <li>这是有序列表的第一行</li>
            <li>这是有序列表的第二行</li>
            <li>这是有序列表的第三行</li>
        </ol>
    </body>
</html>
```
![img](\image\2.png)

##### 标签属性
每一个标签对应其“特点”
```html
<input name="username" type="text" class="login">
```
其中name、type、class都被称为标签属性
其中**name**为标识名，其特点
1. 唯一，即不可重名
2. 第一个元素必须是字母，即`7qxy`错误
3. 对大小写敏感 `username`和`UserName`不同

#### 常用表格元素
```html
<table border="1">
    <tr>
        <th>学号</td>
        <th>姓名</td>
    </tr>
    <tr>
        <td>1759126</td>
        <td>qxy</td>
    </tr>
    <tr>
        <td>1759132</td>
        <td>lzy</td>
    </tr>
</table>
```
<table border="1">
    <tr>
        <th>学号</td>
        <th>姓名</td>
    </tr>
    <tr>
        <td>1759126</td>
        <td>qxy</td>
    </tr>
    <tr>
        <td>1759132</td>
        <td>lzy</td>
    </tr>
</table>

其中`<tr> </tr>`代表一行
<th></th>代表表头单元格
<td></td>代表单元格
border是table的一个属性，代表边框宽度



#### 表单元素
最重要的，用于数据的提交
```html
<form>
    username:<input type="text" name="username"/>
    <br/><!--换行符号-->
    年龄：
    <select>
        <option>15岁以下</option>
        <option>18岁以下</option>
        <option>我已成年</option>
    </select>
    <br/>
    其他信息：
    <textarea></textarea>
</form>
```
<form>
    username:<input type="text" name="username"/>
    <br/><!--换行符号-->
    年龄：
    <select>
        <option>15岁以下</option>
        <option>18岁以下</option>
        <option>我已成年</option>
    </select>
    <br/>
    其他信息：
    <textarea></textarea>
</form>
其中input-`输入框`，对应username后的输入框 select-`列表框`，对应年龄后的复选框，与option组合使用，option代表框里的一个个选项
textarea-`多行文本输入框`，对应其他信息后的多行输入框

#### 其他元素
* `<img></img>`
示例：
```html
<img src="C:\Users\QW\Desktop\html\.vscode\java web\image"></img>
```
<img src="C:\Users\QW\Desktop\html\.vscode\java web\image\13.jpg"></img>
其中src中是图片地址，使用img的height，width属性调整图片大小
示例：
```html
<img 
height="50" width="50" src="C:\Users\QW\Desktop\html\.vscode\java web\image\13.jpg"></img>
```
<img 
height="50" width="50" src="C:\Users\QW\Desktop\html\.vscode\java web\image\13.jpg"></img>
* `<div></div>`
页面分块，即将页面逻辑上分成一块块区域
与样式组合使用
* `<span></span>`
行内分块
与样式组合使用
* `<sup></sup>`
上标
    ```html
    x<sup>5</sup>
    ```
    x<sup>5</sup>
* `<sub></sub>`
下标
    ```html
    C<sub>3</sub>
    ```
    C<sub>3</sub>
* `<br/>` 也可写作`<br>`
换行符，用于换行
    ```html
     hello<br/>world
     ```
    hello<br/>world
* `<hr/>` 也可写作`<hr>`
画一条水平线
    ```html
    <hr/>
    ```
    <hr/>
* `<video></video>`和`<audio></audio>`
展示视屏或音频，html5支持
    ```html
    <video width="320" height="240" controls>
        <source src="movie.mp4" type="video/mp4">
        <source src="movie.ogg" type="video/ogg">
    </video>
    ```
<!--
### CSS
给标签添加属性，以描述网页的**排版布局**
#### 定义样式表的三种方式
1. 外部样式表文件
2. 内部样式表文件
3. 元素中样式表文件
如果对于一个标签，定义了多层样式表，优先级由1到3递增
##### 元素内样式表
<a style="color:blue;font-size:12px;"></a>
-->
### javaScript
1. 基于对象和事件驱动并具有安全性能的解释型脚本语言
2. 不需要进行编译
3. 直接嵌入HTTP页面
4. 把2静态页面转变成支持用户交互并相应用事件的动态页面，仅进行前端的交互。
```html
<html>
    <head>  
            <!--页面中直接嵌入js-->
            <script language="javascript">
                    alert("hello");
                    </script>
            <!--链接外部嵌入js-->        
        <script language="javascript" src="hello.js"></script>
    </head>
    <body>  
        <!---js作为url，写在href中，要加javascript：-->
        <a href="javascript:a=1;b=2;alert('a+b='+(a+b))">touch me</a>
        <!---js作为事件处理程序，写在onclick中，不用加javascript：-->
        <input type="button" value="js作为事件处理" onclick="a=1;b=2;alert('a+b='+(a+b))"/>
    </body>
</html>
```

#### js数据类型
* 数值型：整型、浮点型
* 字符型：需要用单引或者双引括起来
* 布尔型：true和false，也可以用0表示false，非0表示true

#### js变量
* 命名规则
1. 由字母、数字或者下划线组成，第一位不可以为数字（除此之外，空格、加号等等等均不允许出现）
2. 不能使用js中的关键字

与java、c++变量的命名规则一致
* 变量声明
1. 使用前必须先声明
    >var a,b
2. 可在声明时赋值
    >var a=100,b=200
3. 若是未声明，直接赋值也是可以的，js会隐式声明
    >c=100 //此时会进行隐式声明
4. 允许重复声明
    >var a=100
    var a="abc" //a的值为“abc”
5. 重复声明时，若没有为变量赋值，则变量的值不变
    >var a=100
    var a //a的值还是100

#### js变量的数据类型
js是弱类型语言，不强制变量的数据类型，由输入的数据决定
>var a=100  //a为整型
var a="abc" //a为字符串类型

#### js变量的作用域
1. 全局变量（定义在所有函数外）
2. 局部变量（定义在函数体内）

#### 字符串运算
>x = "hello"+"world"
//x的值为helloworld
x = 2+3+"abc"
//x的结果为5`5abc`
//2+3为整型相加，结果为5,5+"abc"，数据类型不同，5转换成字符串类型，即5abc
x="abc"+2+3
//x结果为abc23
//"abc"+2,数据类型不同。统一为字符串，结果为"abc2","abc2"+3，数据类型不同，统一为字符串，结果为"abc23"

#### 其他类型转换为数字
* 字符串：若内容为数字，则转为对应数字，否则转为NaN
* 逻辑值：true转为1，false转为0
* undefined：转为NaN
* null：转为0
* 其他对象：转为NaN
#### 其他类型转换为数字
* 数值：转为对应字符串
* 逻辑值：true转为"true'，false转为"fasle"
* undefined：转为"undefined"
* null：转为"null"
* 其他对象：有toString()方法，转换为对应返回值，佛足额转换为"undefined"
#### 其他类型转换为逻辑值
* 数值：0和NaN转为false，否则true
* 字符串：长度为0转为false，否则为true
* undefined：转为false
* null：转为false
* 其他对象：true
#### 条件分支语句
* if语句
* switch语句
* for循环
* while循环
* do/while循环
* continue语句
* break语句
与java一致
#### js函数
```html
<script>
function do(){
	//todo...
}
</script>
```
```html
<html>
<head>
    <script>
     function displayName(){
         document.getElementById("show").innerHTML="qxy";
     }    
    </script>
</head>
<body>
    <h1 id="show">我要显示姓名</h1>
    <input id="bt1" type="button" value="try" onclick="displayName()"/>
</body>
</html>
```
#### js数组
```js
var cars=new Array();
cars[0]="ford";
cars[1]="Audi";
```
或者
```js
var cars=new Array("ford","Audi");
```
**js中超范围引用不报错，显示为undefined**

### jsp
与服务器交互
基本构成：
1. 指令标签
2. 注释
3. 嵌入java代码
4. jsp动作标签

#### 指令标签
```
<%@ directive attribute=“value” attribute=“valueN” …… %>
```
其中directive：指令名称
attribute：属性名称
value：属性值
#### jsp常用指令及主要功能
>* page:设置整个页面的静态属性
>* include:向当前页面插入一个静态文件的内容，可以是jsp或者html
>* taglib指令：使用标签库定义新的自定义标签，属于jsp中的启用定制行为


#### javaBean
>* 遵循特定的写法：
>   * 这个java类必须有一个无参的构造函数
>   * 属性必须私有化
>   * 私有化属性通过public类型的方法暴露给其他程序，方法命名需遵循一个规则。
>* 相关的jsp标签
>   * <jsp:useBean>:查找或实例化一个javaBean组件；存在则，返回引用；不存在，则创建；
>   * <jsp:setProperty>:用于在jsp页面设置一个javaBean组件的属性
>   * <jsp:getProperty>:用于在jsp页面获取一个javaBean组件的属性
#### jsp小汇总
##### 三大指令
* page
* include
* taglib
##### 四大语法
* 注释
> <!--我是html注释-->
> * 我是html注释,可是我已经把自己注释掉了
> * <% //我是java注释>
> * <%-- 我是jsp注释-->

*jsp注释最强大，注释的内容即使在源文件也不显示*

* 声明
    >* <%! %>  用于声明**全局变量**，其实就是jsp生成类的成员变量
    *jsp本质还是java*
    >* <% %>  **局部变量**，脚本中调用
* 表达式
    >* <%= a%> 即输出a的值到网页端
* 脚本段
    >* <% int a=;go();%>
    可以内嵌java代码
##### 七大动作
* jsp:forward(请求转发)
    ><jsp:forward page="content.jsp"></jsp:forward>
* jsp:plugin(插入插件)
    ><jsp:plugin type="" code=""></jsp:plugin>
    在浏览器中播放或显示一个对象
* jsp:useBean （见前）
* jsp:setProperty  （见前）
* jsp:getProperty  （见前）
* jsp:include   (见前)
* jsp:param （传递参数）
    ><jsp:param name="" value=""/>
##### 九大内置对象
* 四大作用域对象
    * pageContext
    >作用域:一次页面
    * request
    >作用域：一次请求，一次表单提交

    request.getParameter();
    * session
    >作用域：客户端与服务器建立的一次会话，即账号登录以后，经过页面跳转，数据账号信息仍然保留

    方法|返回值|说明
    ----|----|-----
    getAttribute(String name)|Object|获得指定名字的属性
    getAttributeNames()|Enumeration|获得session中所有属性对象
    getCreationtime()|Long|获得session对象的创建时间
    getId()|String|获得session对象的唯一编号
    * application
    >作用域：多个客户端与服务器会话共享，即应用程序在服务器中运行的全局信息。不可以存放个人信息，会被共享。

    方法|说明
    ---|---
    getInitParameter(String name)|返回一个已命名的参数值
    getAttributeNames()|返回所有已定义的应用程序初始化名称的枚举
* 三大打酱油对象
    * page  页面对象
    * exception 例外对象
    * config 配置对象
* 二大输出对象
    * out 输出对象，向客户端发送数据的对象，文本级
    * response  向客户端的响应对象，组织方式底层，不建议使用

    response。sendRedirect();

#### servlet和jsp的区别
1. servlet是客户请求和业务请求的中间角色，而jsp还要承担显示层的一些任务
2. servlet需要调用servlet api接口处理HTTp请求，jsp页面直接使用内置对象
3. servlet的使用需要进行配置，jsp则由容器直接识别，直接**编译为servlet**进行处理

#### servlet的生命周期
init()->service()->destroy()
单实例，多线程
每次调用servlet并不会重新创建servlet，而是调用其service()方法进行服务

1. init()
在servlet生命周期中，仅执行一次，在服务器装入servlet时执行
2. service()
servlet的核心，包含两个方法
    * doGet()：处理get请求
    * doPost()：处理post请求
3. destory():
    * 在服务器执行reload时执行
    * 关掉服务器或者在指定的时间间隔后调用


#### 同一用户不同页面共享数据：
四种方法：
1. cookie技术
2. sendRedirect()跳转
3. 隐藏表单提交(form)
4. session技术

#### 什么是过滤器
servlet过滤器是客户端与目标资源间的中间层组件，用来拦截**客户端**的请求与相应信息。
可以理解为防火墙
可以配置多个过滤器，按照一定的顺序串行执行（以过滤器的`.java`名字排序，字典顺序决定执行顺序）
#### 接口与生命周期，与servlet相似
1. init()初始化，由容器调用，对于每一个Filter实例，只调用一次
2. doFilter:类比service()，进行过滤处理
3. destroy():过滤器生命周期结束调用此方法，释放资源

### 驱动程序接口Driver
用于数据库连接
```java
Class.forName("com.mysql.jdbc.Driver")
//8.0版本的驱动包，需要使用 "com.mysql.cj.jdbc.Driver"
```
#### 连接数据库的步骤
1. 加载JDBC驱动程序
2. 创建数据库连接
3. 执行sql语句
4. 获得查询结果
5. 关闭连接
# 数据库其他内容 to be continue...


### Spring框架
未补充完全
* Context
    1. 继承了BeanFactory类
* AOP模块
* Dao模块
    1. 提供JDBC的抽象层
    2. 简化了数据库厂商的异常错误
    3. 大幅减少了代码的编写
    4. 提供了对声明式和编程式事务的支持
* Spring Coare
    1. Spring的核心容器
#### Sping的配置结构
jar包->tlb标签库->applicationContext.xml文件
再到Spring应用项目

#### 补充
1. 关于Bean的配置操作（Bean可以理解为对象，使对象的关联关系变得清晰）
IOC：反转资源获取的方向
DI：依赖（容器）注入，和IOC一个意思
#### 配置Bean
* 配置形式
    1. 基于XML文件的方式
    2. 基于注解的方式
* Bean的配置方式
    1. 通过全类名（反射）
        >Bean中必须有无参的构造器
        通过ID获取实例
    2. 通过工厂方法（静态工厂方法&&实例共擦方法）
    3. FactoryBean
* 依赖注入
    1. 属性注入
    >提供setter方法
    2. 构造器注入
    >使用构造器注入属性可以指定参数的位置和类型
    注入时直接在value中添加属性，一般为字面值，若不为字面值（包括特殊符号），使用![CDATA]
    ```xml
    <constructor-arg type="java.lang.String">
		<value><![CDATA[<ShangHai……>]]></value>
	</constructor-arg>
    ```

* IOC容器
    1. BeanFactory：IOC容器的基本实现
    2. ApplicationContext:提供更多的高级特性，是BeanFactory的接口（几乎所有场合都使用这个）
* ApplicationContext的两个实现类
    1. ClassPathXmlApplicationContext：
    从类路径加载配置文件
    2. 


* Bean之间的引用
```xml
<!-- bean之间的引用 -->
<bean id="person" class="com.test.Person">
	<property name="name" value="qxy"></property>
	<property name="age" value="18"></property>
	<!-- 可以使用property的ref建立Bean之间的引用关系 -->
	<property name="car" ref="car2"></property>
</bean>
 
<!-- 内部Bean引用 -->
<bean id="person1" class="com.test.Person">
	<property name="name" value="bxy"></property>
	<property name="age" value="8"></property>
	<property name="car">
		<bean class="com.test.Car">
			<property name="brand" value="fute"></property>
		</bean>
	</property>
</bean>
```
支持级联属性
```xml
<!-- bean之间的引用 -->
<bean id="person" class="com.test.Person">
	<property name="name" value="qxy"></property>
	<property name="age" value="18"></property>
	<!-- 可以使用property的ref建立Bean之间的引用关系 -->
	<property name="car" ref="car2"></property>
	<!-- 为级联属性赋值 -->
	<property name="car.price" value="250000"></property>
</bean>
```
```xml
<!-- 测试如何配置集合属性 -->
<bean id="person3" class="com.listTest.Person">
	<property name="name" value="jacklove"></property>
	<property name="age" value="20"></property>
	<property name="cars">
		<list>
			<ref bean="car"/>
			<ref bean="car2"/>
		</list>
	</property>
</bean>

<!-- 配置Map集合 -->
<bean id="person4" class="com.listTest.NewPerson">
	<property name="name" value="mapPerson"></property>
	<property name="age" value="20"></property>
	<property name="cars">
		<map>
			<entry key="AA" value-ref="car"></entry>
			<entry key="BB" value-ref="car2"></entry>
		</map>
	</property>
</bean>
```

Spring IOC容器可以自动装配Bean，需要的仅仅是在<bean>的autowire属性里指定自动装配的模式。
1. byType
2. byName
3. 构造器：不推荐使用

##### bean属性的继承,可覆盖
``` xml
<!-- bean配置的继承 parent -->
	<bean id="address" class="com.autoWire.Address" p:city="Xuzhou" p:street="yunlong"></bean>
	<bean id="address2" parent="address" p:street="tongshan"></bean>
```
也可以继承抽象bean
```xml
	<!-- bean配置的继承 abstract -->
	<bean id="address" class="com.autoWire.Address" p:city="Xuzhou" p:street="yunlong" abstract="true"></bean>
	<bean id="address2" parent="address" p:street="tongshan"></bean>

```
抽象bean不可以被实例化，若bean的class属性不存在，则必须为抽象Bean

##### bean之间的依赖关系
即在一个Bean中引用别的Bean

##### bean的作用域
默认为单例，多次创建都为同一个bean
容器创建时，构造方法已经创建

##### 使用外部属性文件
数据库连接的属性创建方式
1. 以bean的形式写在spring的配置文件中，但是bean多了，后期想要修改很麻烦
2. 写在外部属性中，然后在spring配置文件中导入外部bean
spring提供了BeanFactory后置处理器，允许用户将Bean配置部分内容外移到属性文件中
```xml
	<!-- 导入属性文件 要引入context命名空间 -->
	<context:property-placeholder location="classpath:db.properties"></context:property-placeholder>
	
	<bean id="dataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource">
		<!-- 使用外部属性文件的属性 -->
		<property name="user" value="${user}"></property>
		<property name="password" value="${password}"></property>
		<property name="driverClass" value="${driverclass}"></property>
		<property name="jdbcUrl" value="${jdbcurl}"></property>
	
	</bean>
```

##### Spring表达式语言：SpEL
支持运行时查询和操作对象图的强大的表达语言
语法类似于EL：SpEL使用#{...}作为定界符，所有在大框号中的字符都将被认定为SpEL
SpEL为bean的属性进行动态赋值提供了遍历
通过SpEl可以实现：
1. 通过bean的id对bean进行引用
2. 调用方法及引用对象中的属性
3. 计算表达式的值
4. 正则表达式的匹配
```xml
<bean id="address" class="com.spel.Address">
		<!-- 使用spel赋字面值 -->
		<property name="city" value="#{'Beijing'}"></property>
		<property name="street" value="wudaokou"></property>
	</bean>
	
	<bean id="car" class="com.spel.Car">
		<property name="brand" value="Audi"></property>
		<property name="price" value="50000"></property>
		<!-- 说那个spel引用类的静态属性 -->
		<property name="typePerimeter" value="#{T(java.lang.Math).PI*80}"></property>
	</bean>
	
<!-- 	<bean id="person" class="com.spel.Person"> -->
		<!-- 使用spel来应用其他的Bean --> 
<!-- 		<property name="car" value="#{car}"></property> -->
 		<!-- 使用spel来应用其他的Bean的属性 --> 
<!-- 		<property name="city" value="#{address.city}"></property> -->
		<!-- 在spel中使用运算符 --> 
<!-- 		<property name="info" value="#{car.price>300000?'金领':'白领'}"></property> -->
		
<!-- 		<property name="name" value="lucifer"></property> -->
<!-- 	</bean> -->
	
	<bean id="person" class="com.spel.Person" p:name="newLucifer" p:car="#{car}" p:city="#{address.city}" p:info="#{car.price>300000?'金领':'白领'}"></bean>
```

##### IOC容器中Bean的生命周期方法
Spring IOC容器可以管理Bean的生命周期，Spring允许在Bean生命周期的特定点执行定制的任务
Spring IOC容器对Bean的生命周期进行管理的过程：
1. 通过构造器或工厂方法创建Bean实例
2. 为Bean的属性设置值和对其他Bean的引用
3. 调用Bean的初始化方法
4. Bean可以使用
5. 容器关闭时，调用Bean的销毁方法

即构造->set方法->init方法->...->销毁
在Bean的声明里可以指定Bean的初始化和销毁方法，属性：init-method和destroy-method

可以通过Bean的后置处理器，来在初始化之前和之后进行操作。
```xml
<bean id="car" class="com.beansCircle.Car" init-method="init"  destroy-method="destory" p:brand="Audi" p:price="5000000"/>


<!-- 实现BeanPostProcessor接口，并具体提供 
	Object postProcessorBeforeInitialization(Object bean,String beanName):init-method之前被调用
	Object postProcessorAfterInitialization(Object bean,String beanName):init-method之后被调用
	
	bean:bean实例本身
	beanName：IOC容器配置的bean的名字
	返回值：是实际上返回给用户的那个Bean，注意：可以在以两个方法中修改返回的bean，甚至返回一个新的bean
	
-->

<!-- 配置后置处理器 ：不需要配置i的，IOC容器自动识别是一个BeanPostProcessor -->
<bean class="com.beansCircle.MyBeanPostProcessor"></bean>
```
MyBeanPostProcessor.java
```java
public class MyBeanPostProcessor implements BeanPostProcessor {

	@Override
	public Object postProcessAfterInitialization(Object bean, String beanName) throws BeansException {
		// TODO Auto-generated method stub
		
		System.out.println("postProcessbefore:"+bean+"postProcessbeforeName:"+beanName);
		if("car".equals(beanName)) {
			//...
		}
		return bean;
	}

	@Override
	public Object postProcessBeforeInitialization(Object bean, String beanName) throws BeansException {
		// TODO Auto-generated method stub
		System.out.println("postProcessbefore:"+bean+"postProcessAfterName:"+beanName);
		Car car = new Car();
		car.setBrand("ford");
		return car;
	}

}
```

## 工厂方法创造bean
1. 静态工厂方法
```java
/**
 * 静态工厂方法：直接调用某一个类的静态方法就可以返回Bean的实例
 * @author QW
 *
 */
public class StaticCarFactory {
	private static Map<String, Car>cars=new HashMap<String, Car>();
	static {
		cars.put("audi", new Car("audi", 500000));
		cars.put("ford", new Car("audi", 300000));
	}
	public static Car getCar(String name) {
		return cars.get(name);
		
	}
}
```
```xml
	<!-- 通过静态工厂方法来配置bean，注意不是配置静态工厂方法实例，而是配置bean实例 -->
	<!-- class:指向静态工厂方法的全类名
		 factory-method:指向静态工厂方法的名字
		 constructor-arg：如果工厂方法需要传入参数，则使用constructor-arg来配置参数
	-->
	<bean id="car1" class="com.factory.StaticCarFactory"
	factory-method="getCar">
		<constructor-arg value="audi"></constructor-arg>
	</bean>
```
2.  实例化工厂方法
```java
/**
 * 实例工厂方法：即先创建工厂本身，再调用返回Bean的实例
 * @author QW
 *
 */
public class InstanceCarFactory {
	private Map<String,Car>cars = null;
	
	public InstanceCarFactory() {
		cars = new HashMap<String,Car>();
		cars.put("audi", new Car("audi",500000));
		cars.put("ford", new Car("ford",300000));
		
	}
	public Car getCar(String brand) {
		return cars.get(brand);
	}
}
```

```xml
<!-- 通过实例工厂方法来配置Bean -->
	<!-- factory-bean：指向实例工厂方法的Bean
		 factory-method:指向静态工厂方法的名字
		 constructor-arg：如果工厂方法需要传入参数，则使用constructor-arg来配置参数
	-->
<bean id="carFactory" class="com.factory.InstanceCarFactory">
</bean>
<bean id="car2" factory-bean="carFactory" factory-method="getCar">
	<constructor-arg value="ford"></constructor-arg>
</bean>
```
### 通过FactoryBean配置字Bean
```java
/**
 * 自定义FactoryBean需要实现FactoryBean接口
 * @author QW
 *
 */
public class CarFactoryBean implements FactoryBean<Car>{
	
	
	private String brand;
	public void setBrand(String brand) {
		this.brand=brand;
	}
	
	//返回Bean的对象
	@Override
	public Car getObject() throws Exception {
		// TODO Auto-generated method stub
		return new Car(brand,500000);
	}
	//返回Bean的类型
	@Override
	public Class<?> getObjectType() {
		// TODO Auto-generated method stub
		return Car.class;
	}
}
```

```xml
	<!-- 通过factoryBean来配置Bean的实例 -->
	<!-- 
		class:指向FactoryBean的全类名
		property：配置FactoryBean的属性
		但实际返回的却是Factory的getObject()方法返回的实例
	 -->
	<bean id="car" class="com.factoryBean.CarFactoryBean">
		<property name="brand" value="BMW"></property>
	</bean>
```

### 之前均是通过xml来配置bean，下面来看基于注解配置bean的方式
* 组件扫描：Spring能够从classpath下自动扫描，侦测和实例化具有特定注解的组件
* 特定组件包括：
	-@Component：基本注解，标识一个受Spring管理的组件
	-@Resposity：标识持久层组件
	-@Sevrice：标识服务层（业务层）组件
	-@Controller：标识表现层组件
	（也可以交换，不过不建议）
对于扫描到的组件，Spring有默认的命名策略：使用非限定类名，第一个字母小写，也可以在胡姐中通过value属性值标识组件的名称。
使用注解后，还需要在Spring的配置文件中声明<context:component-scan>:
	-base-package属性指定一个需要扫描的基类包，Spring容器将会扫描这个基类包里及其子包中的所有类
	-当需要扫描多个包时，可以用逗号隔开
	-如果仅希望扫描特定的类而非基包下的所有类，可以使用resource-pattern属性过滤特定的类
	-<context:include-filter>子节点要包含的目标类
	-<context:exclude-filter>子节点表示要排除在外的目标类
	-<context:component-scan>下可以拥有若干个<conetxt:include-filter>和<context:exclude-filter>子节点



2. 综述及标签的使用
java web和java ee
    java web：jsp、servlet开发web程序
    java ee：包含功能比较多，大规模、分布式、健壮的网络应用

java web
    前置技术：
        前端：HTML、CSS、js
        后端
        数据库
    后续：
        框架

jsp：
    本质上就是servlet
    静态网页+java=jsp网页
tomcat：web项目的容器
     java本来的运行：
        java源程序--(jdk)-->.class字节码文件--（jre）-->运行
     java web：
        java类、jsp、servlet类---->可运行的web项目---->部署到tomcat上即可运行        
什么是http：
请求转发：
    request.getRequestDispatcher("login.jsp").forward(request,response);
值传递：
    request.setAttribute("key",value);
    request.getAttribute("key").toString();
    每一次访问产生一个request对象
    不能在页面之间传值，可以转发
session:生命周期，一次会话，从打开网页到关闭，包含多次请求。一次客户端对应一个session
    销毁：关闭网页，长时间不与网页交互，默30分钟。
    session.setAttribute("key",value)
    seesion.getAttribute("key")
application:
    级别最高，不同客户端使用同一个application
    生命周期：每一个应用对应一个application，tomcat的启动与关闭
    统计登录个数
servlet:
    处理请求的逻辑
    在servlet中使用session，application
    HttpSession s = request.getSession(); 
    ServletContext application=this.getServletContext();    

    生命周期方法：
        tomcat启动：构造方法->init()
        客户端访问：doget()
        tomcat关闭：destory()
    service:
        无论调用doget还是dopost都首先调用service    
        super.service（arg0,arg1）调用doget,dopost方法

    配置方式:
        1.注解
        2.web.xml（WEB——INF）（方便修改）
        <servlet>
            <servlet-name></servlet-name>
            <servlet-class></servlet-class>
        </servlet>
        <servlet-mapping>
            <servlet-name></servlet-name>
            <url-pattern></url-pattern>
        </servlet-mapping>

    重定向&&请求转发
        请求转发：url不改变，request数据可以传输
            request.getRequestDispatcher("login.jsp").forward(request,response);
        重定向：服务器端无法处理，返回response，使客户端访问新的页面。
            新请求，故request对象改变，不能通过request传值
            response.sendRedirect("login.jsp")
    
    page：当前对象，=this
        生命周期：仅在本页面有效
        page < request < session < application
    pageContext:页面容器
        pageContext.getOut()
        pageContext.getRequest()
        pageContext.getResponse()
        pageContext.getServletContext() //application
        pageContext.getSession()
        pageCOntext.setAttribute("key",value,scope)

    解决乱码：
        request.setCharacterEncoding("utf-8")

    页面包含：
        jsp统一页面头部尾部
        引入：
            <jsp:include page="head.jsp"></jsp:include>    
    项目绝对路径：
        <%=request.getContextPath()%>/css/style.css  
        要注意客户端路径
        客户端绝对路径：http://localhost:8080/
        服务器端绝对路径: http://localhost:8080/web04/

    单例模式：
        public static JDBCUtil{
            //静态实例
            public static JDBCUtil instance = new JDBCUtil();
            //构造方法私有化
            private JDBCUtil(){

            }

        }          

    MVC分例结构：
        model：数据模型
        view：视图，jsp
        controller：servlet，控制层  

    企业级分层：
        web层：jsp，servlet
        service层:业务逻辑处理
        Dao层：单纯的数据库增删改查      
    

    el表达式：（放在jsp代码块，而非java代码块）
     仅做取值                        
     可以做简单运算
        ${empty list }
        ${60+70 }
     简单对象：
        可以从page、request、session、application中取数据
        ${requestScope.number}
        ${number} 从page到application依次取出 
     复杂对象：
        User u=new User("中国","134","男",false);
        request.setAttribute("user",u);

        ${user.username}  一定要提供标准的get的方法
    map集合：
        Map<String,String>map=new HashMap<String,String>();
		map.put("name","齐祥遥");
		map.put("age","13");
		request.setAttribute("map", map);

        ${map.name }<br/>
	    ${map.age }<br/>
    List集合：
        List <User>list=new ArrayList<User>();
		list.add(new User("pangzi","qwe",13,"男",false));
		list.add(new User("pangzi1","qwe",13,"男",false));
		list.add(new User("pangzi3","qwe",13,"男",false));
		list.add(new User("pangzi4","qwe",13,"男",false));
		list.add(new User("pangzi5","qwe",13,"男",false));
		request.setAttribute("list",list);    

        ${user.username }<br/>
        ${map.name }<br/>
        ${map.age }<br/>
        ${list[3].username }<br/>
        ${empty list }<br/>
        ${60+70 }
jstl:
    标签库
    引入：
        <%@ taglib uri="http://java.sun.com/jsp/jstl/core" prefix="c" %>
    使用：
        设置值：
            <c:set var="username" value="qxy" scope="request"></c:set>
             相当于使用request设置attribute
        输出值：
            <c:out value="bxy"></c:out>
        移出值：
            <c:remove var="username"/>
        条件语句：
            <c:if test="${isAdmin }">
            success
            </c:if>
        分支语句：
            <c:choose>
            <c:when test="${isAdmin }">true</c:when>
            <c:otherwise>false</c:otherwise>
            </c:choose>
        循环语句：
            <c:forEach var="i" begin="1" end="10">
            ${i }
            </c:forEach>
          从list中取数据：
            <%
            List <User>list=new ArrayList<User>();
                    list.add(new User("pangzi","qwe",13,"男",false));
                    list.add(new User("pangzi1","qwe",13,"男",false));
                    list.add(new User("pangzi3","qwe",13,"男",false));
                    list.add(new User("pangzi4","qwe",13,"男",false));
                    list.add(new User("pangzi5","qwe",13,"男",false));
                    request.setAttribute("list",list);
                    %>

            <c:forEach items="${list }" var="u">
            ${u.username }<br/>

            </c:forEach>  
    ajax：
        不进行页面跳转的情况下，对服务器发出请求

filter：过滤器
    权限控制
    请求发出->层层过滤，调用filter
    服务器响应->层层过滤（相反），调用filter
    过滤谁的请求？
    过滤那种请求？
    <dispatcher></dispatcher>
监听器：
    request session application的变化
    HttpServletRequest HttpSession ServletContext
单点登录：
    session集合管理
路径问题（相对路径和绝对路径）
客户端路径 http://ip:port/
服务器端路径http://ip:port/项目名
request.getContextPath()这就是相对路径了
