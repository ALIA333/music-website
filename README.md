# music

#### 介绍
springboot音乐播放网站



## 项目简介

​        此音乐网站使用的是SpringBoot进行设计的，并且采用前后端分离的方式，具有如下的优点：实现真正的前后端解耦，易发现bug，可以快速定位是谁的问题，不会出现互相踢皮球的现象。在大并发情况下，我可以同时水平扩展前后端服务器。减少后端服务器的并发/负载压力。其次，使用SpringBoot减少了大量的开发时间并提高了生产力，也避免了编写大量的样本代码、注释和XML配置。解决了spring中以来反射，反射又影响进程的情况。也解决了Spring中太依赖设计模式的情况，同时SpringBoot可以很好地支持分布式应用。

​        使用Vue做前端是因为它是一个轻量级的框架，简单易学。能够进行双向数据绑定自动对页面中的某些数据的变化做出同步的响应。本音乐网站的客户端和管理端使用 **Vue** 框架来实现，服务端使用 **Spring Boot + MyBatis** 来实现，数据库使用了 **MySQL**。

​        由于歌太大了，只留下了一首周杰伦的听妈妈的话。

<br/>

## 项目功能

- 音乐播放
- 用户登录注册
- 用户信息编辑、头像修改
- 歌曲、歌单搜索
- 歌单打分
- 歌单、歌曲评论
- 歌单列表、歌手列表分页显示
- 歌词同步显示
- 音乐收藏、下载、拖动控制、音量控制
- 后台对用户、歌曲、歌手、歌单信息的管理



## 用到的技术

### 后端

**SpringBoot + MyBatis + MySQL**

### 前端

**Vue + TypeScript + ElementPlus + vue-echarts+ vue-router+ vuex + Axios**

<br/>

## 运行流程

### 1、修改配置文件

1）创建数据库
将 `music-website/music-server/sql` 文件夹中的 `tp_music.sql` 文件导入数据库。

2）修改用户名密码
修改 `music-website/music-server/src/main/resources/application.properties` 文件里的 `spring.datasource.username` 和 `spring.datasource.password`；

### 4、启动项目

- **启动管理端**：进入 music-server 文件夹，运行下面命令启动服务器

```js
// 方法一
./mvnw spring-boot:run

// 方法二
mvn spring-boot:run // 前提装了 maven
```

- **启动客户端**：进入 music-client 目录，运行下面命令

```js
npm install // 安装依赖

npm run serve // 启动前台项目
```

- **启动管理端**：进入 music-manage 目录，运行下面命令

```js
npm install // 安装依赖

npm run serve // 启动后台管理项目
```
