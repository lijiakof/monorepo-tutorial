# Monorepo 入门指南

## 什么是 Monorepo
Monorepo 是一种项目代码管理方式，是 Monolithic Repository 的缩写，是一种多项目单仓库的项目管理方式，这种方式有助于简化代码共享、版本控制、构建和部署等方面的复杂性，并提供更好的可重用性和协作性。

## Monorepo vs Monolith vs Multirepo

* Monolith 单仓库巨石应用
* Multirepo 多仓库多项目应用
* Monorepo 单仓库多项目应用

## Monorepo 使用场景

## Monorepo 方案

## 如何创建 Monorepo 项目

### 简单项目
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

### 复杂项目
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

### npm vs yarn vs pnpm vs lerna

