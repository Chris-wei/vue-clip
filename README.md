# vue-clip

> vue图片裁减压缩

# 效果图
   ![效果图](http://upload-images.jianshu.io/upload_images/6633377-72a12831c84f3f13.gif?imageMogr2/auto-orient/strip)

# 项目描述
> 基于vue的一款图片裁剪压缩工具，可以将用户上传的图片进行最小尺寸压缩，压缩完成后不大于100k，并转化成base64格式，可以直接放入img标签中，可以在控制台看出图片压缩信息
   ![压缩信息](http://upload-images.jianshu.io/upload_images/6633377-3c5c4111e4df639b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# 项目依赖
> cropperjs 第三方的一个裁剪库
> exif      获取图片资源的一个库，用于解决ios下图片翻转的问题

# 项目核心js
> 核心js放在 /src/static/ 下的 clipper.js
> 里面代码注释也挺详细，可以根据实际情况自己改造

# 项目demo
> demo放在 hello.vue 下面
> 调用方法是直接给input[file]控件，添加change事件，并调用methods中的change方法，这里要传event对象
> change方法接收两个参数，第一个是event对象，第二个参数是一个对象，resultObj表示要展示的结果img对象，aspectRatio表示宽高比，另外参数可以根据实际情况添加，主要参考[cropper文档说明][1]

# 项目运行
> 直接 npm install 安装依赖，然后 npm run dev

ps：可以结合我这篇文章一起看看 [基于vue的移动端图片裁剪压缩](http://www.jianshu.com/p/82dbf309f9b1)
## Build Setup

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

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


  [1]: http://blog.csdn.net/qq727013465/article/details/51823231