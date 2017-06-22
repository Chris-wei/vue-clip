# vue-clip

> vue图片裁减压缩

# 项目描述
> 基于vue的一款图片裁剪压缩工具，可以将用户上传的图片进行最小尺寸压缩，压缩完成后不大于100k，并转化成base64格式，可以直接放入img标签中

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