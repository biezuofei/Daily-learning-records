# Npm 

##Npm is usually scripts

	设置npm的registry 
	1.原npm地址
	npm config set registry http://registry.npmjs.org 
	2.设置国内镜像
	a.通过config命令
	npm config set registry https://registry.npm.taobao.org 
	npm info underscore （如果上面配置正确这个命令会有字符串response）
	b.命令行指定
	npm --registry https://registry.npm.taobao.org info underscore 
	c.编辑 ~/.npmrc 加入下面内容
	registry = https://registry.npm.taobao.org
	3.使用nrm管理registry地址
	a.下载nrm
	npm install -g nrm
	b.添加registry地址
	nrm add npm http://registry.npmjs.org
	nrm add taobao https://registry.npm.taobao.org
	c.切换npm registry地址
	nrm use taobao
	nrm use npm
	搜索镜像: https://npm.taobao.org
	建立或使用镜像,参考: https://github.com/cnpm/cnpmjs.org
	
	vue 安装
	npm install --global vue
	npm install --global vue-cli
	
	vue init webpack demo
	npm install -D vuex babel-runtime

//全局安装
npm install -g webpack
//安装到你的项目目录
npm install --save-dev webpack
