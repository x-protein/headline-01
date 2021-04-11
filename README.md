# 利用VUE完成头条项目

## 使用脚手架创建项目

### 什么是脚手架？

Vue CLI 是一个基于 Vue.js 进行快速开发的完整系统

- 通过 @vue/cli 实现的交互式的项目脚手架
- Vue CLI 致力于将 Vue 生态中的工具基础标准化。它确保了各种构建工具能够基于智能的默认配置即可平稳衔接

## 脚手架的安装下载

如果没有安装Vue CLI，打开小黑窗输入如下命令下载：

(下载的是全局包，下载一次即可，后期在任何目录中都能直接使用脚手架创建项目)

```sh
可以使用下列任一命令安装这个新的包：
npm install -g @vue/cli
# OR
yarn global add @vue/cli
```

用这个命令来检查其版本是否正确：

```sh
vue --version
```

![image-20210410202452287](https://i.loli.net/2021/04/10/SfVrPcj5iW9ny1e.png)

## 使用脚手架创建项目

### 在命令行中输入以下命令创建Vue项目

```
vue create 项目名称
```

![image-20210410203638677](https://i.loli.net/2021/04/10/jMk2zv1QliyIScU.png)

### 选择安装的预设

第一步：`> Manually select features`

![image-20210410202832229](https://i.loli.net/2021/04/10/TVNo81EdKqhbXyO.png)



第二步： 

- (*) Babel         :    ES6转ES5
- (*) CSS Pre-processors         :        css预处理器

![image-20210410203051406](https://i.loli.net/2021/04/10/zrIws2NgeEauPZ8.png)

![image-20210410203106543](https://i.loli.net/2021/04/10/124x5U3tCgWS7X9.png)



第三步：项目中选择`less`做为预处理器

![image-20210410203238958](https://i.loli.net/2021/04/10/u7DO9plN6wWdTR1.png)



第四步：`> In dedicated config files`

![image-20210410203434404](https://i.loli.net/2021/04/10/aDYA1OzNVleb6fu.png)



第五步：`? Save this as a preset for future projects? (y/N) N`

![image-20210410203507590](https://i.loli.net/2021/04/10/HX3Ys6IJFSuPKaG.png)



第六步：出现  `$ cd headline`  和` $ npm run serve`  表示创建成功

![image-20210410203806615](https://i.loli.net/2021/04/10/KZgtBmaVzLcP2j6.png)

### 运行脚手架生成的项目



第一步：用`cd headline`切换路径

![image-20210410203949223](https://i.loli.net/2021/04/10/6IwGuYAPpyLRVKc.png)



第二步：运行脚手架`npm run serve`

![image-20210410204142094](https://i.loli.net/2021/04/10/3xOjNGKX8itrbLF.png)



第三步：将URL地址复制到浏览器运行即可，切记需要联网

![image-20210410204307511](https://i.loli.net/2021/04/10/8pMUTgrRiKzcClt.png)



第四步：出现下面的界面则说明运行成功

![image-20210410204509560](https://i.loli.net/2021/04/10/5FOqMNkfLoEnKsc.png)



## 调整项目初始化结构

*默认的目录结构不满足开发的需求，需要新增调整目录结构*

### 删除初始化的默认文件

1. 删除 `src/components/HelloWorld.vue`文件

   ![image-20210410205001892](https://i.loli.net/2021/04/10/psWkiZcMTy9A3dr.png)

2. 在`App.vue`中移除对HelloWorld的引入及使用

   ![image-20210410205215110](https://i.loli.net/2021/04/10/fAnySIUWQzPZj3r.png)

### 新增调整我们需要的目录结构

1. 在`src`文件里面文件目录如下

   ```sh
   --src               
   --src/apis          目录：放置封装的接口方法
   --src/App.vue       
   --src/assets        
   --src/commponents   目录：放置封装组件
   --src/main.js       
   --src/router        目录：放置路由模块
   --src/utils         目录：放置公共的工具模块
   --src/styles        目录：放置全局样式
   --src/views         目录：放置页面组件
   ```

2. `src`初始化结构目录

   ![image-20210410214113409](https://i.loli.net/2021/04/10/uVRIgZHFeQsKcBp.png)

### 调整之后的目录结构

![image-20210410214822045](https://i.loli.net/2021/04/10/m9faNnFbDJYoSUe.png)

### 引入全局的重置样式

  ？？？？？？



## 添加登录单文件组件

### 创建登录单文件组件，并添加简单的结构

在`views`目录中添加`login.vue`单文件组件

![image-20210411004620754](https://i.loli.net/2021/04/11/znwvQRXGZsJ2HpV.png)





