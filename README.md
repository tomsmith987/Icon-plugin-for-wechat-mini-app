# 欢迎使用随手图标字体微信小程序插件

**[随手图标字体小程序](https://github.com/tomsmith987/Icon)插件的图标全部是矢量图表，主要是满足开发者使用字体图标的需求，其中约包括675个图标，如果该插件得对您有帮助，欢迎给我一个好评**

## 引入指南
直接在[微信公众平台](https://mp.weixin.qq.com/)添加插件中提出申请即可(添加最下方管理员微信，通知他您已发送申请，以及申请的小程序名，管理员会在一天内审批通过)，插件的appid为：wx0a3a3dc8953ae613

在json文件中配置hand-icon插件
```
  "plugins": {
        "myPlugin": {
            "version": "1.0.0",
            "provider": "wx0a3a3dc8953ae613"
        }
   },
   "usingComponents": {
        "hand-icon": "plugin://myPlugin/hand"
   }
```
[点我跳转github上的官方文档](https://github.com/tomsmith987/Icon "跳转到github官方文档")
## 样例展示

#### 代码演示：
基础用法
type属性：选择图标基本样式
```html
<hand-icon type="cc-amex"></hand-icon>
```
size属性：图标大小调节
```html
<hand-icon type="cc-amex" size="lg"></hand-icon>
<hand-icon type="cc-amex" size="2x"></hand-icon>
<hand-icon type="cc-amex" size="3x"></hand-icon>
<hand-icon type="cc-amex" size="4x"></hand-icon>
<hand-icon type="cc-amex" size="5x"></hand-icon>
```
class属性：用户自定义class选择器
```html
/*wxml*/
<hand-icon type="hand-o-up" class="my-class"></hand-icon>
```


```css
/*wxss*/
.my-class{
    color:red;
    font-size:100rpx;
}

```
spin属性：是任意图标旋转
```html
<hand-icon type="circle-o-notch"  spin="{{true}}"></hand-icon>  
<hand-icon type="refresh"  spin="{{true}}"></hand-icon>  
<hand-icon type="spinner"  spin="{{true}}"></hand-icon>
```
rotate和flip属性：图标旋转与翻转
```html
<hand-icon type="hand-o-up"></hand-icon>
<hand-icon type="hand-o-up" rotate="90"></hand-icon>
<hand-icon type="hand-o-up" rotate="180"></hand-icon>
<hand-icon type="hand-o-up" rotate="270"></hand-icon>
<hand-icon type="hand-o-up" flip="horizontal"></hand-icon>
<hand-icon type="hand-o-up" flip="vertical"></hand-icon>
```
图标嵌套使用：其中inverse是颜色翻转属性
```html
/*wxml*/
<view>
        <hand-icon stack="stack">
            <hand-icon type="square-o" slot="out" stack="stack-2x"></hand-icon>
            <hand-icon type="twitter" slot="in" stack="stack-1x"></hand-icon>
        </hand-icon>
    </view>

    <view>
        <hand-icon stack="stack">
            <hand-icon type="circle" slot="out" stack="stack-2x"></hand-icon>
            <hand-icon type="flag" slot="in" stack="stack-1x" inverse="{{true}}"></hand-icon>
        </hand-icon>
    </view>

    <view>
        <hand-icon stack="stack">
            <hand-icon type="square" slot="out" stack="stack-2x"></hand-icon>
            <hand-icon type="terminal " slot="in" stack="stack-1x" inverse="{{true}}"></hand-icon>
        </hand-icon>
    </view>
</view>
```
```css
/*wxss*/
.red-color {
    color:#a94442;
}
```
图标支持的icon和名称见下图  
![](https://github.com/tomsmith987/README_IMAGE/blob/master/icon/icon.png)


感谢大家使用本插件，欢迎大家也使用随手团队开发的**随手练英语小程序**，利用零碎时间提升英语水平，从而升职加薪，走上迎娶白富美的道路。  
![](https://github.com/tomsmith987/README_IMAGE/blob/master/icon/hand_english_qrcode.jpg)


意见反馈和相关支持请大家添加**小助手微信号（victoria415000）**，小助手会拉你进群，同众多开发者沟通交流。  
![](https://github.com/tomsmith987/README_IMAGE/blob/master/icon/service_qrcode.jpeg)






备注：  
所有标志图标都分别是其所有者的注册商标。  
使用这些商标并不代表该插件拥有它们。  
商标只应用在被提及相应的公司或产品时使用。  
该插件中的部分代码和图标源自于Font Awesome。  

