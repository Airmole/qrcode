# qrcode
二维码生成接口，可以定制内容、尺寸、前景色、背景色及透明度

## 请求方式
http get

##请求参数

参数  | 说明 | 类型  | 是否必需  
---|---|---|---
c | content | 二维码内容 如：http://m.nuomi.com | R
s | size | 大小，每像素几个点 1,2,3,4,5,6.... | 否 默认7
bc | backgroud_color | 背景色&透明度 rgba 逗号分开 | 否 默认白色 255255,255,0
fc | froreground_color | 前景色&透明度 rgba 逗号分开 | 否 默认黑色 0,0,0,0

## 返回
直接输出图片 

## 存在的坑

不知道是不是因为我php换了新版本的问题。之前是php5.x只有c参数确实是必需的，升级到php7.2以后，必须四个参数都带上才能显示出来二维码。
