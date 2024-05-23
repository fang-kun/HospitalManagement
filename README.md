# 医院管理系统+AI聊天问诊

医院管理系统 (his) 采用 Servlet + JSP 的架构进行设计，AI聊天问诊 (chatthymeleaf-test-master) 采用Springboot + Thymeleaf 的架构实现。两个程序均可独立运行，且分别上传至两个仓库。

<br>

其中，医院管理系统与AI聊天问诊是独立的两个程序，两者通过前端融合实现最终的系统效果。

<br>

**本仓库仅含医院管理系统 (his) 。**

AI聊天问诊 (chatthymeleaf-test-master) 仓库为：[AI-Chat-Consultation](https://github.com/fang-kun/AI-Chat-Consultation)

<br>

## 集成开发环境

- JDK：corretto-11
- Tomcat：8.5.75
- Maven：3.8.4
- Idea：2021.3.1
- Navicat：15

## 基础搭建方法

1. 将两个项目Git到本地Idea工作空间，并导入Idea配置好上述JDK环境。在Navicat的3306端口下的连接，导入his项目下的 his.sql 文件。

<br>

2. 配置 his 项目。在Idea中配置 Tomcat，选择自己下载好Tomcat的本地路径进行配置。确保Tomcat的配置中的Deployment正确导入了his项目（如下图），启动Tomcat。

![](D:\IdeaProjects\his\WebRoot\Images\mdPic.jpg)

<br>

3. 配置 chatthymeleaf-test-master 项目（请确保在此之前Maven已配置在Idea中）。打开 pom.xml 文件，右键->Maven->Reload Project，引入依赖。启动Springboot启动类。

<br>

4. 两个项目正常启动后，浏览器运行 http://localhost:8080/his/
