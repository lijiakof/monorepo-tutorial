# Monorepo 入门指南

* npm init
* npm init -w packages/utils
* package.json
  * "workspaces": [ "packages/*" ]
* npm create vue@latest -w packages
  * 请输入项目名称：app
  * .vscode 移动到更目录
* 更目录 package.json
  * "scripts": { "dev": "npm run dev -workspaces" }
* npm i
