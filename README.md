# Mini-Pro
微信小程序学习

* [小程序社区-文章类](http://www.wxapp-union.com/portal.php)  
* [小程序窝-小问题类](http://www.xcxwo.com/thread/index)  
* [Qdaily 小程序 开发过程](https://www.zhihu.com/question/50907897/answer/140010208)  
*   [一起脱去小程序的外套 - 微信小程序架构解析](https://mp.weixin.qq.com/s/3QE3g0NmaBAi91lbrihhVw)
*   [微信小程序开发资源汇总](https://github.com/justjavac/awesome-wechat-weapp)
*   [微信小程序开发系列文章](https://www.cnblogs.com/yexiaochai/p/9346043.html)
*   [知乎：如何入门微信小程序开发，有哪些学习资料？](https://www.zhihu.com/question/50907897/answer/128494332)
*   [掘金小程序 Tag](https://juejin.im/tag/%E5%BE%AE%E4%BF%A1%E5%B0%8F%E7%A8%8B%E5%BA%8F)

## 学习小程序大致分三个阶段  
1）概念建立阶段，通过浅阅[官文文档](https://developers.weixin.qq.com/miniprogram/dev/framework/)，阅读社区教程、文章完成  
2）知识结构充实阶段，通过阅读他人的demo源码，在本地运行，调试修改，带着问题学习是这个阶段的主要特征，要善用搜索引擎，善于在群内提问  
3）开发修行阶段，投入到实际的项目开发中去，在实践中提高认识，并提出新的问题，改进既有的开发方案，编写小程序类库、工具等  



## 小程序开源开发框架介绍

### WePY

微信小程序问世没多久，大家发现用原生小程序语法开发，开发体验和效率真的不尽如人意。WePY 此时横空出世，彼时 WePY 的目的，是让小程序开发更贴近传统 H5 框架开发，支持引入 npm 包，支持组件化开发和 ES Next 新特性。

1.  开发模式：更符合现有 MVVM 框架的开发模式，类 Vue，节省上手成本
2.  组件化开发：支持组件嵌套、循环、组建通信等
3.  npm 包管理：处理了 npm 包依赖问题
4.  ES Next：语法更现代，提升开发体验
5.  细节优化：setData 性能优化（脏检测）、事件传参、编译器支持、Mixin

正是由于 WePY 解决了原生微信小程序的开发痛点，到目前为止，WePY 也是小程序上层框架中使用方最多的。很多开发者都是基于 WePY 开发微信小程序的，微信官方后续的一些性能优化和特性支持也有 WePY 的影子。

[wepy-cli](https://www.npmjs.com/package/wepy-cli) 的周下载量月度平均都维持在 1000 以上，远远领先于同类 cli 工具，star 数 12k+，也正如官网所说，是最受欢迎的小程序框架。使用 WePY 框架的接入，更是达到了上千家。

### mpvue

随着小程序接入量的猛增，业界也在不断地对小程序开发体验进行尝试。2018 年 3 月，美团点评发布了一个名叫 mpvue 的小程序框架。mpvue 是一套定位于开发小程序的前端开发框架，其核心目标是提高开发效率，增强开发体验。

mpvue 是基于 Vue 的 Runtime（Vue Runtime 除了我们知道的 Web 平台之外，还有 Weex），相比 WePY，mpvue 的语法更接近 Vue 语法，对于有 Vue 基础的童鞋，可以无缝切换到小程序的开发，省下了学习小程序语法的时间。

### Taro

Taro 是 2018 年 6 月，由京东凹凸实验室出品的一款号称多端统一的框架。这里的端，指的是 Web、App（React Native、Weex）、小程序。Taro 主打「一次编写，多端运行」，是继 WePY 和 mpvue 之后，在多平台上做到了更彻底的一款框架。
