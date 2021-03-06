# cooking

[![Build Status](https://travis-ci.org/ElemeFE/cooking.svg?branch=master)](https://travis-ci.org/ElemeFE/cooking) [![Coverage Status](https://coveralls.io/repos/github/ElemeFE/cooking/badge.svg?branch=master)](https://coveralls.io/github/ElemeFE/cooking?branch=master) [![npm](https://img.shields.io/npm/dm/cooking.svg?maxAge=2592000)](https://www.npmjs.com/package/cooking) [![npm](https://img.shields.io/npm/v/cooking.svg?maxAge=3600)](https://www.npmjs.com/package/cooking) [![Dependency Status](https://david-dm.org/elemefe/cooking.svg)](https://david-dm.org/elemefe/cooking) [![devDependency Status](https://david-dm.org/elemefe/cooking/dev-status.svg)](https://david-dm.org/elemefe/cooking#info=devDependencies)

> 更易上手的前端构建工具

## 文档
http://cookingjs.github.io

## 介绍
在项目开发中每次创建一个新项目都要去安装一堆的如 babel、webpack、eslint 等依赖，其实多数情况下每个项目的依赖和版本都是相同的；如果用 webpack 做构建工具的话，配置又较为繁琐。所以 cooking 将为你做这些事

- 全局安装开发依赖，无需每个项目重复安装
- 提供 webpack 的预配置（内置 ES6、dev server、hotload 特性），同时提供一套简洁的配置参数和函数
- 扩展配置和依赖模块化，只在需要的时候才安装且引入到配置中
- 完全兼容已有 webpack 的配置文件，除了未提供的依赖需要自己安装，其它情况下使用一致
- 内置脚手架工具

## 安装

运行环境
- Node.js 4+
- npm 3+
- Python 2.7.x

```shell
npm i cooking -g
```

## 快速开始
Step 1. 创建一个 vue 项目 （将自动下载 vue 项目脚手架，只需下载一次）
```shell
> cooking create my-project vue
> cd my-project
```

Step 2. 开始开发
```shell
> cooking watch
```

## 常见问题

### Cannot find module 'xxx'

确保使用 NPM 3.0 及其以上版本

### permission denied

不推荐使用 root 权限安装及执行 cooking，如果强制使用请在每次执行是带上 `--allow-root` 参数，或者推荐做法是将 node_modules 目录的权限改成当前用户。

```shell
# 找到自己的全局 node_modules 的路径
sudo chown -R 用户名 /usr/local/lib/node_modules
```

# License
[MIT](https://github.com/ElemeFE/cooking/LICENSE)
