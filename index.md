## Welcome to GitHub Pages

### 李凤琼20182123045

```
用例名称	Security System
用例说明	管理者在完成登录操作后，可以进行总览，设置安全政策，发布安全公告，查看dependabot警报，代码扫描警报等一系列操作
参与者	管理员
元素	Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts，Set up a security policy，View security advisories，Configuration，Set up code scanning，Draft，Published，Closed，Automatically detect，Security analysis from the marlcetplace
关系	管理员对于Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts是依赖关系
建模思路	1.泛化关系，Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts是overview的几种形式，Overview，Security policy，Security advisories，Dependabot alerts，Code scanning alterts继承了overview的结构，行为和关系；Code scanning alterts和Set up code scanning也为泛化关系
2.包含关系，管理者进入Dependabot alerts之后可以进行Configuration操作，所以Dependabot alerts和Configuration为包含关系；管理者进入Security policy进行Set up a security policy操作，俩者也为包含关系
3.扩展关系，当发布了安全公告时，才发生Draft，Published，Closed这些操作，所以它们均是View security advisories的扩展关系
```
