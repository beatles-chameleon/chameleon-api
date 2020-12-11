# chameleon-api  [![version](https://img.shields.io/npm/v/chameleon-tool.svg?style=flat)](https://www.npmjs.com/package/chameleon-api) [![Build Status](https://travis-ci.org/beatles-chameleon/chameleon-api.svg?branch=master)](https://travis-ci.org/beatles-chameleon/chameleon-api)

# 说明
本仓库为chameleon的api的相关代码，chameleon 支持大量基础API，对外提供统一的接口，以模块的方式引入chameleon-api进行使用。
接口查看及扩展等请见文档： https://beatles-chameleon.github.io/doc/api/api.html


例如:
``` javascript
import cml from 'chameleon-api'

cml.showToast({
  message: 'Hello world!',
  duration: 1000
})
```

## 分支说明  
分支对应版本号  例如1.0.8-alpha.4  对应版本外网1.0.8-alpha.4  内网 3.0.8-alpha.4

## 如何开发
结合cml-dome仓库进行开发调试

使用npm link的方式将本地仓库与cml-demo依赖建立链接

实现cml-demo依赖本地chameleon-api进行开发

## 单元测试与覆盖率测试
```
npm i 
npm run test
npm run cover
```

## 发布正式版本:

修改package.json中version

sh publish.sh

## 发布alpha版本:

修改package.json中version

sh publish.alpha.sh