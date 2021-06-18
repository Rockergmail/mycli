1. 如何变成全局包？
   1. 创建可执行的脚本
   2. 配置package.json的bin字段
   3. npm link 链接到本地 npm unlink

/Users/rocker/.nvm/versions/node/v10.19.0/bin/mycli -> /Users/rocker/.nvm/versions/node/v10.19.0/lib/node_modules/mycli/bin/mycli
/Users/rocker/.nvm/versions/node/v10.19.0/lib/node_modules/mycli -> /Users/rocker/vhost/myproject/mycli

2. 脚本名称是基于package.json的name，当然可以在bin字段设置别的名称
3. 规划：
   1. 命令行+交互 commander + chalk + inquirer
   2. 下载模板 download-git-repo
   3. 根据用户的选择动态生成内容 metalsmith

1. 模板准备：文件如何组织，不同类型的项目【另外一个大课题】
2. 命令行和交互设计【commander+ chalk + inquier + ora】
3. 下载【主要是调用github的api以及download库】
