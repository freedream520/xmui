<div align=center><a href="https://github.com/monw3c/xmui" target="blank"><img src="https://github.com/monw3c/xmui/blob/master/docs/imgs/logo.png"/></a></div>  

# XMUI  

[![Version](https://img.shields.io/npm/v/x-m-ui.svg)](https://www.npmjs.com/package/x-m-ui) [![Downloads](http://img.shields.io/npm/dm/x-m-ui.svg)](https://www.npmjs.com/package/x-m-ui) [![License](https://img.shields.io/npm/l/x-m-ui.svg?style=flat)](https://opensource.org/licenses/MIT) [![TravisCI](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://travis-ci.org/XadillaX/x-m-ui)  

基于vue 2+ ，为公司产品打(zao)造(lun)的(zi)可复用UI组件，适用于 移动 和 部分PC 端，其中包括 基础组件 和 应用组件，目前 组件 和 文档 在不断完善中。


## 特性

- 基于 [Vue](http://vuejs.org/)`>=v2.1.4` 开发的可复用 UI 组件，并且可随产品需要扩展
- 使用Vue官方的工作流，支持 ES6
- 一系列线上产品都在使用中
- 关于SEO问题推荐使用插件 [prerender-spa-plugin](https://github.com/chrisvfritz/prerender-spa-plugin)

## 浏览器支持

- 适用于 移动 和 部分PC 端(Chrome,safari,IE9+等)

## 开发  
> 全局引入 -- 在 webpack 入口文件 main.js 中如下配置：

``` bash
# 安装
cnpm install x-m-ui --save  

# 引入css
import 'x-m-ui/package/xmui.min.css'  

# 引入xmui.min.js
import xmui from 'x-m-ui'  

# 注入到vue
Vue.use(xmui)
```

> 按需引入 -- 在 入口文件 main.js 或 组件内 中如下配置：

``` bash
# 全局组件 main.js引入
import Toast from 'x-m-ui/package/comps/components/toast'
Vue.prototype.$toast = Toast

# 一般组件
import xmButton from 'x-m-ui/package/comps/components/button'
import xmButtonGroup from 'x-m-ui/package/comps/components/buttongroup'
import xmModal from 'x-m-ui/package/comps/components/modal'
...

components: {
    xmButton,
    xmButtonGroup,
    xmModal
    ...
}
``` 
更多说明，请查看[在线文档](https://monw3c.github.io/xmui/)

## 查看示例  

[在线示例](https://monw3c.github.io/xmui/dist/)  

## 组件列表
- [x] 按钮
- [x] 标签
- [x] 加载更多
- [x] 搜索框
- [x] 单元格
- [x] 表单
- [x] 网格和图标
- [x] flexbox
- [x] Modal
- [x] Toast
- [x] Loading
- [x] 工单流程
- [x] skeleton骨架
- [ ] 轮播
- [x] ActionSheet
- [ ] 左右滑菜单
- [ ] 时间选择器
- [ ] 标签页
- [x] 导航栏(顶部)
- [x] 标签栏(底部)

## 关于如何构建 Vue 组件库的文章，有兴趣的朋友可了解一起探讨 

[如何基于 Vue 2 写一套 UI 库](http://gitbook.cn/gitchat/activity/5a5df169462f9b46f3418520)

## 贡献

在此不一一感谢所有付出脑力体力的同仁，如有疑问，请与我们联系   
如果你在使用时遇到问题，或者有好的建议，欢迎给我们提 [Issue](https://github.com/monw3c/xmui/issues) 或 [Pull Request](https://github.com/monw3c/xmui/pulls)
