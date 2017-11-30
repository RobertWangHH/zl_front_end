## 志力信息科技有限公司后台管理前端技术文档
### 浏览器兼容要求
<p align="center">
    <img src="https://img.shields.io/circleci/project/vuejs/vue/dev.svg" alt="Build Status">
    <img src="https://img.shields.io/codecov/c/github/vuejs/vue/dev.svg" alt="Coverage Status">
    <img src="https://img.shields.io/npm/dm/vue.svg" alt="Downloads">
    <img src="https://img.shields.io/npm/v/vue.svg" alt="Version">
    <img src="https://img.shields.io/npm/l/vue.svg" alt="License">
    <img src="https://img.shields.io/badge/chat-on%20discord-7289da.svg" alt="Chat">
    <br><br>
    <img src="https://saucelabs.com/browser-matrix/vuejs.svg" alt="Sauce Test Status">
</p>


```gantt
    title 项目开发流程
    section 项目确定
        需求分析       :a1, 2016-06-22, 3d
        可行性报告     :after a1, 5d
        概念验证       : 5d
    section 项目实施
        概要设计      :2016-07-05  , 5d
        详细设计      :2016-07-08, 10d
        编码          :2016-07-15, 10d
        测试          :2016-07-22, 5d
    section 发布验收
        发布: 2d
        验收: 3d
```

## 技术栈
本项目使用者为公司内部人员，不必兼容到IE低版本<br>
>  vue2 + vuex + vue-router + webpack + ES6/7 + fetch + less + flex + svg +element-ui（较为前沿的技术）<br><br>
>  layui(如果要兼容IE8浏览器的话推荐这个,这是一款采用自身模块规范编写的前端框架，遵循原生HTML/CSS/JS的书写与组织形式。体积轻盈，组件丰盈，从核心代码到API的每一处细节都经过精心雕琢，非常适合界面的快速开发。)



#layui
![此处输入图片的描述][1]

layui 定义为“经典模块化”，本身也并不是完全遵循于AMD时代，准确地说，她试图建立自己的模式，所以你会看到：

```js
//layui模块的定义
layui.define([mods], function(exports){

  //……

  exports('mod', api);
});

//layui模块的使用
layui.use(['mod1', 'mod2'], function(args){
  var mod = layui.mod1;

  //……

});
```
它具备AMD的影子，又并非受限于commonjs的那些条条框框，layui认为这种轻量的组织方式，比WebPack更符合绝大多数场景。所以她坚持采用经典模块化，也正是能让人避开工具的复杂配置，回归简单。

但是 layui 又并非是Requirejs那样的模块加载器，而是一款UI解决方案，她与Bootstrap最大的不同恰恰在于她糅合了自身对经典模块化的理解。
> 对用户体验比较友好，一个功能是一个js文件，按需加载，不用在初始化的时候就加载很多静态资源。

## 效果演示
#### 示例(该框架部分UI截图，可根据设计另外单独自定义)
#### 提示等配色
![此处输入图片的描述][2]
![此处输入图片的描述][3]
#### 数据表格提供灵活的自定义空间
![此处输入图片的描述][4]
#### 按钮
![按钮][5]
![此处输入图片的描述][6]
#### 时间选择
![此处输入图片的描述][7]
![此处输入图片的描述][8]
## 项目运行

#### 注意：由于涉及大量的 ES6/7 等新属性，node 需要 6.0 以上版本

```
npm install

npm run dev

```


## 说明

>  开发环境  nodejs 6.10.0


## 关于 数据接口 的说明

### 2017-11-24

> 关于数据请求的方式，可以有两种方案，一种是在服务器上部署nodejs-express，中转前端与服务器的数据，
第二种就是前端打包后的静态文件放在服务端项目中，推荐第一种，前后端分离。



# 效果演示
#### 示例(相关UI的截图，并不是本项目的)
<img src="https://raw.githubusercontent.com/bailicangdu/vue2-manage/master/screenshots/manage_home.png"/>



# 目标功能(请打勾)
- [ ] 部门设置
- [ ] 岗位设置
- [ ] 账号管理
- [ ] 权限设置
- [ ] 消息通知
- [ ] 用户管理
- [ ] 会员管理
- [ ] 企业认证
- [ ] 委托查看
- [ ] 需求创建
- [ ] 需求单管理
- [ ] 需求查看
- [ ] 供应商报价查看
- [ ] 供应商签约
- [ ] 合同管理
- [ ] 信用管理


## 确认签字:__________________


  [1]: https://saucelabs.com/browser-matrix/layui.svg
  [2]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/alerts.png
  [3]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/warning.png
  [4]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/table.png
  [5]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/buttons.png
  [6]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/buttons%282%29.png
  [7]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/date1.png
  [8]: http://wh-alibaba-haha.oss-cn-shanghai.aliyuncs.com/work/date2.png