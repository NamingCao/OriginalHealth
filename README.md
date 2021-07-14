# OriginalHealth

## 简介

### 项目介绍
  一款应用于健康管理机构的业务系统，实现健康管理机构工作内容可视化、会员管理专业化、健康评估数字化、健康干预流程化、知识库集成化，
从而提高健康管理师的工作效率，加强与会员间的互动，增强管理者对健康管理机构运营情况的了解。

### 项目技术
  本项目结构上分为表现层、业务层和数据访问层。层次间的依赖关系自下到上。
  前端技术栈采用H5+BootStrap+ElementUI+Vue.js+ajax，使得静态资源风格简约化，对用户友好性较高；
  用Dubbo+Zookeeper+SpringMVC+Spring Security完成分布式架构及权限；使用Git进行版本控制；
  持久层则是用到了MyBatis框架和MySQL数据库。此外，还用到了第三方服务，如阿里云通信服务、七牛云存储服务。
  
### 模块划分
  各模块职责定位：
  1、health_parent：父工程，打包方式为pom，统一锁定依赖的版本，同时聚合其他子模块便于统一执行maven命令
  2、health_common：通用模块，打包方式为jar，存放项目中使用到的一些工具类、实体类、返回结果和常量类
  3、health_interface：打包方式为jar，存放服务接口
  4、health_service_provider：Dubbo服务模块，打包方式为war，存放服务实现类、Dao接口、Mapper映射文件等，作为服务提供方，需要部署到tomcat运行
  5、health_backend：传智健康管理后台，打包方式为war，作为Dubbo服务消费方，存放Controller、HTML页面、js、css、spring配置文件等，需要部署到tomcat运行
  6、health_mobile：移动端前台，打包方式为war，作为Dubbo服务消费方，存放Controller、HTML页面、js、css、spring配置文件等，需要部署到tomcat运行

## 部分展示：
