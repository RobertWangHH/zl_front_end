## 志力信息科技有限公司后台管理前端技术文档


## 技术栈
本项目使用者为公司内部人员，不必兼容到IE低版本<br>
>  vue2 + vuex + vue-router + webpack + ES6/7 + fetch + less + flex + svg +element-ui（较为前沿的技术）<br><br>
>  layui(如果要兼容IE8浏览器的话推荐这个,这是一款采用自身模块规范编写的前端框架，遵循原生HTML/CSS/JS的书写与组织形式。体积轻盈，组件丰盈，从核心代码到API的每一处细节都经过精心雕琢，非常适合界面的快速开发。)



## layui
<p align="center">
    <img src="https://saucelabs.com/browser-matrix/layui.svg" alt="Sauce Test Status">
</p>

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


## Vue

>  vue2 + vuex + vue-router + webpack + ES6/7 + fetch + less + flex + svg +element-ui


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