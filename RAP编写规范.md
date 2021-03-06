#RAP编写规范
##文档目的
* 建立公司后端接口编写规范，降低前后端不必要的沟通成本。
* 通过接口的一致性，确保代码复用。
* 规范输入和输出
##修改记录
<table>
<tr>
	<td>版本</td>
	<td>日期</td>
	<td>内容</td>
</tr>
<tr>
	<td>0.1</td>
	<td>2016年8月25日</td>
	<td>创建接口文档</td>
</tr>
</table>

###项目建立

填写项目名称：
> 请使用客户对这个项目定义的项目名。

填写项目描述：
> 需要写出项目的web工程名，它的主要作用，涉及用到了那些前端表现，例如桌面浏览器，手机浏览器，微信，Android，iOS等。

###模块划分
按微服务的方式将模块分化，一个模块对应一个TabbarItem，例如订单可构成一个模块，通知可构成一个模块，共用部分独立构成一个公用模块。

###页面划分
一个页面所需要的全部接口，归档在一个页面中。如果有引用其它页面的接口，也请写明，务必要体现前端在处理这个页面时，需要调用的所有接口。

###编写接口

####接口详情
填写接口名称：
> 在RESTful架构中，每个网址代表一种资源（resource），所以网址中不能有动词，只能有名词，而且所用的名词往往与数据库的表格名对应。一般来说，数据库中的表都是同种记录的"集合"（collection），所以API中的名词也应该使用复数。
举例来说，有一个API提供动物园（zoo）的信息，还包括各种动物和雇员的信息，则它的路径应该设计成下面这样。

https://xxx.example.com/v1/zoos
https://xxx.example.com/v1/animals
https://xxx.example.com/v1/employees

填写请求类型：
> GET（SELECT）：从服务器取出资源（一项或多项）。
POST（CREATE）：在服务器新建一个资源。
PUT（UPDATE）：在服务器更新资源
DELETE（DELETE）：从服务器删除资源。

填写说明：
> 这里请详细说明这个接口的用途，创建人，创建时间，最后一次修改人，最后一次修改时间。
列出引用该接口的其它页面。
<b>如果此接口不为所属的页面专有，需特别指出引用接口的具体路径，且不填写请求响应参数</b>

返回格式：
> 请默认对象

####请求参数



####响应参数
