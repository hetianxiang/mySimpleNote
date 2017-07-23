# 全局安装
$ npm install <package name> -g
# 范例
$ npm install express -g
# 安装完后现在我们可以用 <code>express</code> 来产生
$ express new app
# 每个组件需要重新安装组件包
$ cd /path/to/the/project
$ npm install <package name>
# 范例
$ npm install express
# 现在就可以用 `var express = require( 'express' );` 来使用 express 这个套件了.
# 删除全局包
$ npm uninstall <package name> -g
# 范例
$ npm uninstall express -g
# 移除路径下的软件
$ cd /path/to/the/project
$ npm uninstall <package name>
# 范例
$ npm uninstall express
# 查找组件
$ npm search <package name>
# 范例
$ npm search express
# 显示全局组件.
$ npm ls -g
# 显示全局组件详细内容.
$ npm ls -gl
# 显示项目组件
$ cd /path/to/the/project
$ npm ls
# 显示项目内组件内容的详细内容
$ cd /path/to/the/project
$ npm ls -l
# 更新全局组件
$ npm update -g
# 更新项目内的组件
$ cd /path/to/the/project
$ npm update
# npm切换淘宝镜像方法
$ npm --registry https://registry.npm.taobao.org install express
# 永久切换
$ npm config set registry https://registry.npm.taobao.org
# 验证是否成功
npm config get registry
