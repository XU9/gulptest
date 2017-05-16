gulpfile.js是gulp项目的配置文件，是位于项目根目录的普通js文件
其实将gulpfile.js放入其他文件夹下亦可）。
说明：命令提示符执行gulp 任务名称；
	编译less：命令提示符执行gulp testLess；
	当执行gulp default或gulp将会调用default任务里的所有任务[‘testLess’,’elseTask’]

一、
使用gulp-less插件将less文件编译成css，当有less文件发生改变自动编译less，并保证less语法错误或出现异常时能正常工作并提示错误信息
安装：命令提示符执行 npm install gulp-less --save-dev
	--save-dev 保存配置信息至 package.json 的 devDependencies 节点。

二、
使用gulp-htmlmin压缩html，可以压缩页面javascript、css，去除页面空格、注释，删除多余属性等操作
安装：命令提示符执行 npm install gulp-htmlmin --save-dev

三、
使用gulp-uglify压缩javascript文件，减小文件大小。
安装：命令提示符执行 npm install gulp-uglify --save-dev

四、
使用gulp-concat合并javascript文件，减少网络请求。
安装：命令提示符执行 npm install gulp-concat --save-dev

五、
使用gulp-imagemin压缩图片文件（包括PNG、JPEG、GIF和SVG图片）。
安装：命令提示符执行 npm install gulp-imagemin --save-dev

六、
使用browser-sync能让浏览器实时、快速响应您的文件更改（html、js、css、sass、less等）并自动刷新页面。
安装：命令提示符执行 npm install browser-sync --savev--dev

	 gulp.watch('src/**/*.less', ['testLess']); //当所有less文件发生改变时，调用testLess任务

     
    Markdown Editing和Markdown Preview 插件

