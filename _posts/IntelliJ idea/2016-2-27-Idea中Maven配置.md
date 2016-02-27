---
layout: post
title: Idea中Maven配置
date: 2016-2-27
summary: maven配置
categories: Idea
thumbnail: lock
author : ychost
orginal : no
tags:
    - Idea
    - Maven
---

#### 1.Maven环境配置
1. ###### 下载[maven](http://mirrors.hust.edu.cn/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.zip)到计算机上，并解压到某目录，假设是C盘
![](/asset/iamges/2016-2-27-1.png)

2. ###### 设置maven的环境变量，将maven根目录设置为环境变量M2_HOME，将%M2_HOME%/bin添加到Path变量里面。
![](/asset/iamges/2016-2-27-2.png)    
<br/>
![](/asset/iamges/2016-2-27-3.png)

3. ###### 测试Maven安装结果 mvn -v
![](/asset/iamges/2016-2-27-4.png)

#### 2.Idea2015 中Maven的相关设置
1. ###### 切换IDEA中默认的Maven路径 File->Setting->BuildTools ->Maven
![](/asset/iamges/2016-2-27-5.png)

2. ###### 设置依赖自动导入 Maven->Importing
![](/asset/iamges/2016-2-27-6.png)

#### 3.使用IDEA创建maven 的Java Web
1. ###### 选择Create from archetype -> maven-archetype-webapp
![](/asset/iamges/2016-2-27-7.png)

2. ###### 填写相关信息
![](/asset/iamges/2016-2-27-8.png)
 Next  
 ![](/asset/iamges/2016-2-27-9.png)
 点击Finish
 ![](/asset/iamges/2016-2-27-10.png)

3. ###### 会自动下载所需依赖，等待下载完成
![](/asset/iamges/2016-2-27-11.png)

4. ###### 相关设置  
   打开File->Setting->Modules，按下图设置
  ![](/asset/iamges/2016-2-27-12.png)
5. ###### 配置Tomcate
![](/asset/iamges/2016-2-27-13.png)    
<br />
![](/asset/iamges/2016-2-27-14.png)  
<br/>
![](/asset/iamges/2016-2-27-15.png)     
<br/>
 点击确定  
 ![](/asset/iamges/2016-2-27-16.png)   

6. ###### 目录结构
![](/asset/iamges/2016-2-27-17.png)   

7. ###### 启动Tomcate
![](/asset/iamges/2016-2-27-18.png)     
<br/>
![](/asset/iamges/2016-2-27-19.png)   

#### 注：
  	所有的配置均在pom.xml里面设置如

  ![](/asset/iamges/2016-2-27-20.png)   


#####  详细设置，请参考 [Maven教程](http://www.yiibai.com/maven/)
