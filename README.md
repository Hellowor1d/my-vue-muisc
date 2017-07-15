# my-vue-music

> study vue-music

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

# 根据 vue-cli 生成基本项目模板，然后改造进而学习 vue-music 项目，熟悉vue2项目的工程实践

### 2017-7-15 项目基本改造
1. 由于`vue-music`项目的 CSS 基于 `stylus`,而`vue-cli`未添加，所以需要手动安装 stylus 和 stylus-loader ；
根据 ![stylus-loader](https://github.com/shama/stylus-loader) 的 github 推荐安装方式：
`npm install stylus-loader stylus --save-dev`

其他变更：
```js
//不检测新文件末尾是否有空行
    'eol-last':0,
//不检测函数括号前加不加空格
    'spcace-before-function-paren':0
```
2. 在 App.vue 文件中，修改template 内容，添加了 “hello 之类内容”；
本节暂时未用到router相关内容，所以都先注释掉；

style 标签中添加`scoped`：表明当前样式只针对当前组件有效，继续设置`lang="stylus" rel="stylesheet/stylus"`,这样stylus-loader就会编译这部分样式了。

