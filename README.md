# xiaochengxu
xiaochengxu for wechat,小程序

## 开始之前
0. 注册开发者：mp.weixin.qq.com
1. 下载开发工具：https://mp.weixin.qq.com/debug/wxadoc/dev/devtools/download.html?t=20161122
2. 下载官方体验小程序源码：https://mp.weixin.qq.com/debug/wxadoc/dev/?t=20161122
3. 用开发工具添加体验小程序，体验
4. 官方简易教程：https://mp.weixin.qq.com/debug/wxadoc/dev/?t=20161122
5. 组件库：https://mp.weixin.qq.com/debug/wxadoc/dev/component/?t=20161122

## 常见问题及解决方案
1. 本地缓存storage,类似localStorage，可以存取改删 String/Object
2. 页面跳转及传值，<navigator url="../detail/detail?name={{item.name}}"></navigator>
3. 跨页面通信，一个方案是：https://github.com/danneyyang/weapp-event
4. 组件化

模版header.wxml
```
<template name="header">
  <view class="page-header">
    <text class="page-header-text">{{title}}</text>
    <view class="page-header-line"></view>
  </view>
</template>
```
使用
```
 <import src="../common/header.wxml" />

 <template is="header" data="{{title: 'start/stopRecord、play/pause/stopVoice'}}"/>

```

