# Angular2-
Angular2环境搭建步骤


安装环境：
		npm i cnpm -g
		cnpm i -g @angular/cli
		ng new myproject
		半路的弹框可选择不下载
		进入项目myproject后
		cnpm install
		在dea的命令栏：ng serve --open
			     或者： npm start
		访问：http://localhost:4200
		
安装完整包：npm i -save @covalent/core


cnpm install @angular/material@2.0.0-beta.
cnpm install  @angular/material@2.0.0-beta.6
cnpm install 

---在命令行中使用命令：ng g c hero-detail  则会在src/app/创建名为hero-detail文件夹，并且里面ts、css的命名方式符合规范。

---安装辅助库：  api  直接在控制台中运行命令：（连网）
	cnpm install angular-in-memory-web-api
	npm install typescript@2.3.4


==dependencies下的这些包是运行本应用的基础，而devDependencies下的只在开发此应用时才用得到。 
通过为install命令添加--production参数，你在产品环境下安装时排除devDependencies下的包，就像这样：
cnpm install my-application --production



---报错1：
	chunk    {0} main.bundle.js, main.bundle.js.map (main) 38.8 kB {2} [initial] [rendered]
	chunk    {1} styles.bundle.js, styles.bundle.js.map (styles) 11.5 kB {3} [initial] [rendered]
	chunk    {2} vendor.bundle.js, vendor.bundle.js.map (vendor) 3.79 MB [initial] [rendered]
	chunk    {3} inline.bundle.js, inline.bundle.js.map (inline) 0 bytes [entry] [rendered]

	ERROR in AppModule is not an NgModule
	解决方法：查看本地的版本：npm ls typescript  然后直接下载  npm install typescript@2.3.4

	
----处理全局变量与本地变量的问题：	 
 Your global Angular CLI version (1.1.2) is greater than your local
version (1.1.1). The local Angular CLI version is used.

To disable this warning use "ng set --global warnings.versionMismatch=false".
	

