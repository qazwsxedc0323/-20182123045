### 李凤琼20182123045

### 用例名称	Security System

### 用例说明	管理者在完成登录操作后，可以进行总览，设置安全政策，发布安全公告，查看dependabot警报，代码扫描警报等一系列操作
### 参与者	管理员
### 元素	
Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts，Set up a security policy，View security advisories，Configuration，Set up code scanning，Draft，Published，Closed，Automatically detect，Security analysis from the marlcetplace
### 关系	
管理员对于Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts是依赖关系
### 建模思路	
1.泛化关系，Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts是overview的几种形式，Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts继承了overview的结构，行为和关系；Code scanning alterts和Set up code scanning也为泛化关系
2.包含关系，管理者进入Dependabot alerts之后可以进行Configuration操作，所以Dependabot alerts和Configuration为包含关系；管理者进入Security policy进行Set up a security policy操作，俩者也为包含关系
3.扩展关系，当发布了安全公告时，才发生Draft，Published，Closed这些操作，所以它们均是View security advisories的扩展关系
### 试论述聚合和组合的异同。
答：聚合描述了整体对象拥有部分对象的关系。组合是聚合的一种形式，它具有强的拥有关系，而且整体与部分的生命周期是一致的。

### 学院公众号中，成绩查询模块可以很方便地使在校学生查询到期末考试成绩，特别是老师将期末成绩提交后，该模块会以弹窗的方式将信息通知到学生，问题：请根据滇池学院微信公众号中，学生成绩查询模块的功能，对该模块进行小组讨论分析，对该功能的类图中以下元素进行必要说明：
### 该功能一共应该包含哪几个类
该功能一共包含成绩类、学期筛选类和成绩下载类。
类名称	类说明
成绩类	显示成绩及其细节
学期筛选类	筛选每个学期的成绩
成绩下载类	下载所有成绩

### 每个类的属性，方法应该是什么，有什么作用，权限该是什么？
学期筛选类：
属性	全部数据	18至20学年所有成绩
	18至19学年上学期	显示该学期内的所有成绩，类型为String，Private属性
	18至19学年下学期	显示该学期内的所有成绩，类型为String，Private属性
	19至20学年上学期	显示该学期内的所有成绩，类型为String，Private属性
	19至20学年下学期	显示该学期内的所有成绩，类型为String，Private属性

方法	查询	查询在该学期内的所有成绩信息
	打印	打印该学期内的所有成绩信息

成绩下载类：
属性	姓名	类型为String，Private属性
	学号	类型为int，Private属性
	学院	类型为String，Private属性
	班级	类型为String，Private属性
	学期	成绩所属学期，类型为String，Private属性
	课程名称	类型为String，Private属性
	课程性质	类型为String，Private属性
	成绩类型	成绩类型为期末总评，类型为String，Private属性
	应修学分	该课程应修学分，类型为String，Private属性
	实修学分	该课程实际所修学分，类型为String，Private属性
	成绩	该课程的成绩，类型为String，Private属性
	绩点	该课程成绩绩点，类型为String，Private属性
	学分绩	该课程学分绩，类型为String，Private属性
方法	保存	保存所有成绩
	发送	发送成绩表

成绩类
属性	考试科目	类型为String，Private属性
	总评成绩	类型为String，Private属性
	学期	类型为String，Private属性
	学科类型	类型为String，Private属性
	应修学分	类型为String，Private属性
	实修学分	类型为String，Private属性
	绩点	类型为String，Private属性
	学分绩	类型为String，Private属性
	平时成绩	类型为Int，Private属性
	作业成绩	类型为Int，Private属性
	期中成绩	类型为Int，Private属性
	期末成绩	类型为Int，Private属性
方法		
