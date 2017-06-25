# ssm
ssm练习项目

* jdbc编程问题

 1. 频繁连接开启与关闭，造成数据库资源浪费，影响性能---数据库连接池
 2. sql在java代码中，硬编码，不利于系统维护---配置文件xml
 3. 参数设置preparedStatement  占位符和参数设置---配置文件xml
 4. 结果集 resultSet获取数据时---自动映射

* Mybatis原理
1. 持久层框架 重点集中在sql上，关系映射，自由灵活生成满足需要的sql语句
2. 输入参数与结果集自动进行输入映射与输出映射java对象

* 项目结构
1. 全局配置文件 SqlMapConfig.xml  数据源、事务等
   
   映射文件(配置映射文件) mapper.xml
2. SqlSessionFactory(会话工厂)  创建SqlSession
   
   SqlSession(会话)  操作curd
   
   Executor(执行器，缓存执行器) SqlSession内部操作
   
   mapped statement(底层封装对象) 数据库、sql语句、输入参数、输出结果类型 
   
开发环境下日志级别要设置成debug




