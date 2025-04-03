# Monorepo 入门指南

## 简单项目
* npm init
* npm init -w packages-simple/utils
  * package name: @monodemo-simple/utils
* 根目录 package.json
  * "workspaces": [ "packages-simple/*" ]
* npm init -w packages-simple/modules
  * package name: @monodemo-simple/modules
* 根目录 package.json
  * "scripts": { "dev": "npm run dev -workspaces" }
* npm i
* npm i @monodemo-simple/utils -w packages-simple/modules

## 复杂项目
* npm init
* npm init -w packages/utils
* 根目录 package.json
  * "workspaces": [ "packages/*" ]
* npm create vue@latest -w packages
  * 请输入项目名称：app
  * .vscode 移动到更目录
* 根目录 package.json
  * "scripts": { "dev": "npm run dev -workspaces" }
* npm i
