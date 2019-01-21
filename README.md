# 多米生活app - 商学院h5

>源码存放在src目录下,config目录为gulp构建工具配置文件，与维护内容基本无关

## 维护说明

> 文章相关部分存放在article-list目录下  

维护主要分为 `文章列表` 和 `文章内容` 的维护  

### 文章列表

列表内容都存放在每一个模块下的`index.html`下, 每一个模块下都有对应的demo示例供参考  

截图说明：  
文章列表由`ul`标签去承载  
其下的每一个`li`都存放着一个文章标题信息  

截图如下：  
![demo-li](https://ws1.sinaimg.cn/large/006tNc79ly1fzebdsosomj30mw0h2ad0.jpg)

### 文章内容

文章内容都存放在每一个模块下的articles目录下, 每一个模块下都有对应的demo示例供参考  

由于文章都采用图片去承载内容，故插入的文章图片存放在src/images目录下(注：使用英文+数字+下划线命名)  

## 项目目录结构

```shell
.
├── README.md
├── config
│   ├── gulp.config.js
│   ├── gulp.dev.js
│   ├── gulp.init.js
│   └── gulp.prod.js
├── gulpfile.js
└── package.json
```

## 开发流程

克隆项目到本地
```
git clone git@github.com:Cui-y/gulp-work.git my-project
cd my-project
rm -rf .git
```

安装依赖

> 要求node版本:  ^6.14.0  ||  ^8.10.0  ||  >=9.10.0

```
yarn install
```

初始化项目目录
```
yarn run init
```

本地开发
```
yarn start
```

语法检查
```
yarn lint --fix
```

## 上线说明

生产上线前需要使用构建工具进行打包, 打包后的资源会存放在dist目录下，之后可以直接将dist下的静态资源进行上传服务器上线

命令行下输入

```shell
yarn build
```

## 协议
MIT
