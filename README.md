## vue-home

>技术点 

用vue社区提供的API，基于vue+vue-cli+vue-router+axios+webpack开发的vue社区webapp

UI用Muse-UI

css用scss，flex布局，rem做移动端适配，最终效果web端移动端都适配。

用localStorage做缓存

> 建议先去社区[注册](https://www.vue-js.com/signup)拿accesstoken登录体验(注册可以直接用github账号，挺快的)

[demo](http://www.hxvin.me/vue-home/dist/)

[点击查看gif动图展示](http://ooytyiziz.bkt.clouddn.com/vue-home.gif)

[项目API](https://www.vue-js.com/api/)
### 手机扫描查看效果
![手机扫描查看效果](https://github.com/Hxvin/vue-home/blob/master/src/assets/1495982696.png)

> 完成功能

- [x] 首页列表
- [x] 下拉加载
- [x] 用户信息（点击头像）
- [x] 主题内容
- [x] 登录功能
- [x] 收藏（取消收藏）主题
- [x] 评论列表
- [x] 点赞（取消点赞）功能
- [x] 消息中心（已读、未读）
- [x] 个人中心
- [x] 发表评论
- [x] 回复评论
- [x] 发布主题（支持markdown编辑且可预览）

> todo功能
- [ ] 左右侧滑
- [ ] 搜索功能
- [ ] 手机横竖屏
- [ ] vuex重构

### 安装运行

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
* 注意`npm run dev` 之后 默认浏览器打开的是http://localhost:8080  请换成http://localhost:8080/vue-home/dist


### 准备开发环境

* $ npm install -g vue-cli 
* $ vue init webpack vue-home

```
? Project name vue-home
? Project description vue-home
? Author afei
? Vue build standalone
? Install vue-router? Yes
? Use ESLint to lint your code? No
? Setup unit tests with Karma + Mocha? No
? Setup e2e tests with Nightwatch? No
```

* $ cd vue-home
* $ npm install
* $ npm run dev

等写完项目后 打包上线
* $ npm run build

>注意：npm run dev 之后 默认浏览器打开的是http://localhost:8080  请换成http://localhost:8080/vue-home/dist
>如果你电脑的8080端口被占用，请congfig/index.js中找到`port: 8080`修改成8081或者其他可用的端口


### 开始动手

#### 项目结构

```
├── build
│   ├── build.js
│   ├── check-versions.js
│   ├── dev-client.js
│   ├── dev-server.js
│   ├── utils.js
│   ├── vue-loader.conf.js
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── config
│   ├── dev.env.js
│   ├── index.js
│   └── prod.env.js
├── dist                  //等写完项目后 $ npm run build 的打包文件
│   ├── index.html
│   └── static
├── index.html            //首页入口文件
├── node_modules
├── package.json          
├── src
│   ├── App.vue           //项目入口文件
│   ├── assets
│   │   ├── 1495982696.png  //手机扫描二维码
│   │   ├── logo.png        //vue logo
│   │   └── sass            //sass通用样式
│   ├── components          //组件
│   │   ├── FooterNav.vue   //底部nav组件
│   │   ├── HeaderBar.vue   //顶部横条
│   │   ├── HeaderTabs.vue  //顶部tabs组件&主页面内容拉取
│   │   └── Hello.vue        
│   ├── main.js             //核心文件 在这里引入了Muse UI 时间过滤器
│   ├── pages               //页面
│   │   ├── content.vue     //帖子内容页面  
│   │   ├── index.vue       //首页
│   │   ├── login.vue       //登录页面
│   │   ├── message.vue     //信息通知页面
│   │   ├── more.vue        
│   │   ├── my.vue          //个人信息页面
│   │   ├── people.vue      //社区用户信息页面
│   │   └── publish.vue     //发布帖子页面
│   ├── router              //路由与组件配置
│   │   └── index.js 
│   └── util                //时间过滤器，转换时间格式
│       └── filter.js
└── static
