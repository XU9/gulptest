gulp的简单使用
==============

## gulpfile.js是gulp项目的配置文件，是位于项目根目录的普通js文件
    如何使用：命令提示符执行gulp 任务名称；
	   编译less：命令提示符执行gulp testLess；
	   当执行gulp default或gulp将会调用default任务里的所有任务[‘testLess’,’elseTask’]

## 安装gulp才能使用以下gulp插件。
>安装：
>（1）在package.json文件下添加gulp模块
>"devDependencies": {
>   "gulp":"*"     
>    // *代表自动匹配版本
>   }
>devDependencies：开发阶段完成集成测试等功能模块依赖
>（2）命令提示符执行 npm install
>注：插件也可采用此安装模式。

## 一、gulp-less
    使用gulp-less插件将less文件编译成css，当有less文件发生改变自动编译less，
    并保证less语法错误或出现异常时能正常工作并提示错误信息
> 安装：命令提示符执行 npm install gulp-less --save-dev

    --save-dev 保存配置信息至 package.json 的 devDependencies 节点。

## 二、gulp-htmlmin
    使用gulp-htmlmin压缩html，可以压缩页面javascript、css，去除页面空格、注释，删除多余属性等
>安装：命令提示符执行 npm install gulp-htmlmin --save-dev

## 三、gulp-uglify
    使用gulp-uglify压缩javascript文件，减小文件大小。
>安装：命令提示符执行 npm install gulp-uglify --save-dev

## 四、gulp-concat
    使用gulp-concat合并javascript文件，减少网络请求。
>安装：命令提示符执行 npm install gulp-concat --save-dev

## 五、gulp-imagemin
    使用gulp-imagemin压缩图片文件（包括PNG、JPEG、GIF和SVG图片）。
>安装：命令提示符执行 npm install gulp-imagemin --save-dev

## 六、browser-sync
    使用browser-sync能让浏览器实时、快速响应您的文件更改
    （html、js、css、sass、less等）并自动刷新页面。
>安装：命令提示符执行 npm install browser-sync --savev--dev


小练习
------
* 请参考本例题使用`gulp-concat`对js文件进行合并
* 插件及配置以及完成，直接添加.js文件并操作
* 你可以尝试`npm uninstall 插件名`来删除插件



