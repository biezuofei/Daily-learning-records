# Npm 

##Npm is usually scripts

	����npm��registry 
	1.ԭnpm��ַ
	npm config set registry http://registry.npmjs.org 
	2.���ù��ھ���
	a.ͨ��config����
	npm config set registry https://registry.npm.taobao.org 
	npm info underscore ���������������ȷ�����������ַ���response��
	b.������ָ��
	npm --registry https://registry.npm.taobao.org info underscore 
	c.�༭ ~/.npmrc ������������
	registry = https://registry.npm.taobao.org
	3.ʹ��nrm����registry��ַ
	a.����nrm
	npm install -g nrm
	b.���registry��ַ
	nrm add npm http://registry.npmjs.org
	nrm add taobao https://registry.npm.taobao.org
	c.�л�npm registry��ַ
	nrm use taobao
	nrm use npm
	��������: https://npm.taobao.org
	������ʹ�þ���,�ο�: https://github.com/cnpm/cnpmjs.org
	
	vue ��װ
	npm install --global vue
	npm install --global vue-cli
	
	vue init webpack demo
	npm install -D vuex babel-runtime

