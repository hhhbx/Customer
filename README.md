# Customer
客户管理系统
功能介绍
  添加客户：添加客户的信息，包含姓名，性别，手机号，邮箱，自我介绍等信息
  客户查询：查询数据库中的所有客户，将查询结果以列表的形式展现出来，可以对列表的客户信息进行编辑和删除操作
  高级搜索：多条件的组合在数据库中进行客户信息的查询，搜索结果以列表的形式给出，可以对列表的客户信息进行编辑和删除
  附加功能：可以分页查看显示客户的信息，每页十条
运用知识：
  数据库基本的查询
  数据库连接池c3p0
  运用dbutil.jar包将数据表单进行一键封装到bean对象中
  利用dbutils.jar对数据库进行增，删，查，改的代码
  jsp的标签库
  javaweb的mvc分层模式
  将servlet的转发、重定向及方法进行封装，这样当设计到多个功能时不用建立多个servlet类
  反射技术
导入jar包
  需要的jar包在项目的lib目录下
  复制到自己项目的lib目录下即可
配置文件
  c3p0-config.xml
建包
  dao：操作数据库
  service：数据库和表单数据的传输中介
  servlet：接收和传输表单数据
  domain：测试项
sql：
  create table t_customer{
  id varchar(50) not null primary key,
  name varchar(50),
  gender varchar(50),
  phone varchar(50),
  email varchar(50),
  decription varchar(50)
  };
