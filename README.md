# xiaochengxu
xiaochengxu for wechat,小程序

## 开始之前
0. 注册开发者：https://mp.weixin.qq.com
1. 下载开发工具：https://mp.weixin.qq.com/debug/wxadoc/dev/devtools/download.html?t=20161122
2. 下载官方体验小程序源码：https://mp.weixin.qq.com/debug/wxadoc/dev/?t=20161122
3. 用开发工具添加体验小程序，体验
4. 官方简易教程：https://mp.weixin.qq.com/debug/wxadoc/dev/?t=20161122
5. 组件库：https://mp.weixin.qq.com/debug/wxadoc/dev/component/?t=20161122
6. 入口，微信-发现-小程序，可以分享给朋友或群聊，可以置顶到消息页。
7. 微信小程序分析服务:http://mta.qq.com/
8. 小程序商店，知晓程序：https://minapp.com/miniapp/，猎豹移动：http://www.duba.com/wxapp/

## 常见问题及解决方案
1. 本地缓存storage,类似localStorage，可以存取改删 String/Object
2. 页面跳转及传值，<navigator url="../detail/detail?name={{item.name}}"></navigator>
3. 跨页面通信，一个方案是：https://github.com/danneyyang/weapp-event
4. 组件化

    如模版：header.wxml
    ```
    <template name="header">
      <view class="page-header">
        <text class="page-header-text">{{title}}</text>
        <view class="page-header-line"></view>
      </view>
    </template>
    ```
    如何使用？
    ```
     <import src="../common/header.wxml" />

     <template is="header" data="{{title: 'start/stopRecord、play/pause/stopVoice'}}"/>

    ```

