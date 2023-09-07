---
authors: lurong
---

# 前端规范

## 软件

1. 编辑器使用 [Visual Studio Code](https://code.visualstudio.com/)
2. 浏览器使用 [Chrome](https://www.google.cn/intl/zh-CN/chrome/)
3. 笔记使用 [Markdown](https://www.runoob.com/markdown/md-tutorial.html)

<!--truncate-->

## 技术栈

<!-- | 技术 | 程度 | 备注 | 顺序 |
| ---- | ---- | ---- | :----: |
| Node | 了解 | 了解 `fs`、`path` 等自带模块的基本用法 | 9 |
| JavaScript | 熟练 | 熟悉 JavaScript 高级，熟练使用 Array、Object、String 等对象自身或原型上的方法 | 1 |
| TypeScript | 熟练 | 熟悉泛型和函数重载，能够通过类型体操初级测试 | 7 |
| CSS | 熟练 | 熟悉各种布局、定位的特点 | 2 |
| Less | 了解 | 了解 Less 的基本语法和变量函数 | 8 |
| Axios | 熟悉 | 了解请求体的格式和拦截器 | 3 |
| Vue | 熟练 | 熟悉组合式 Api 的用法和生命周期 | 4 |
| Vue Router | 了解 | 了解路由的基本用法 | 5 |
| Pinia | 了解 | 了解 Pinia 的基本用法 | 6 |
| Markdown | 熟悉 | 熟悉 Markdown 的语法 | 0 | -->
1. **Node**

    了解 [nvm](https://github.com/coreybutler/nvm-windows) 的基本用法，了解 `fs`、`path` 等自带模块的基本用法，建议学习视频 **[【叩丁狼教育】Node.js零基础入门到高级进阶-20天](https://www.bilibili.com/video/BV13V411b7jH)**，内含 `JavaScript` 和 `Express` 等内容，可自主选择跳过

2. **JavaScript**

    熟悉 JavaScript 高级，熟练使用 Array、Object、String 等对象自身或原型上的方法，建议学习视频 **[尚硅谷JavaScript基础&实战丨JS入门到精通全套完整版](https://www.bilibili.com/video/BV1YW411T7GX)** 和 **[尚硅谷JavaScript高级教程(javascript实战进阶)](https://www.bilibili.com/video/BV14s411E7qf)**，可以按照自身喜好和实力，自主选择和跳过相关章节

3. **TypeScript**

    熟悉泛型和函数重载，能够通过类型体操初级测试，建议学习视频 **[千锋教育前端TypeScript入门视频教程（陆神顶配版TS入门教程）](https://www.bilibili.com/video/BV1H44y157gq)** 和 **[typescript类型体操](https://www.bilibili.com/video/BV1vY41187Tx)**

4. **CSS**

    熟悉各种布局、定位的特点，建议学习视频 **[尚硅谷Web前端零基础入门HTML5+CSS3基础教程丨初学者从入门到精通](https://www.bilibili.com/video/BV1XJ411X7Ud)**

5. **Less**

   了解 Less 的基本语法和变量函数，建议学习视频同 CSS

6. **Axios**

    了解请求体的格式和拦截器，熟记官方 Api 即可，**[Axios 中文网](http://www.axios-js.com/)**

7. **Vue3**

    熟练使用组合式 Api 和生命周期，建议按照 **[Vue 官方文档](https://cn.vuejs.org/guide/introduction.html)** 学习即可

8. **Vue Router**

    了解路由的基本用法，建议按照 **[Vue Router 官方文档](https://router.vuejs.org/zh/introduction.html)** 学习即可

9. **Pinia**

    了解 Pinia 的基本用法，建议按照 **[Pinia 官方文档](https://pinia.web3doc.top/introduction.html)** 学习即可

10. **Markdown**

    熟悉 Markdown 的语法，建议按照 **[菜鸟教程 Markdown 教程](https://www.runoob.com/markdown/md-tutorial.html)** 学习即可

建议学习顺序：

**Markdown** → **JavaScript** → **CSS (Less)** → **Axios** → **Vue3** → **Vue Router** → **Pinia** → **TypeScript** → **Node**

视频和文档仅为建议，可以自主选择其他渠道或者章节进行学习

## Node

1. Node 版本使用 `nvm` 进行管理，统一版本，使用最新的 LTS 版本
    - nvm 下载地址：[nvm](https://github.com/coreybutler/nvm-windows)（Github）
    - 了解 nvm 的基本用法

2. NPM 包管理器统一为 `yarn`，NPM 镜像源统一使用 [NPMMirror](https://registry.npmmirror.com)
    - yarn 安装方式：`npm i yarn -g`
    - npm 更改镜像源：`npm config set registry https://registry.npmmirror.com` 或者 `npx nrm use taobao`
    - yarn 更改镜像源：`yarn config set registry https://registry.npmmirror.com`
    - 了解 yarn 的基本用法，`yarn add` 等同于 `npm install`，`yarn remove` 等同于 `npm uninstall` ...

## 通用格式要求

1. 缩进必须使用空格，均为 4 个空格（可以设置为 Tab 键为 4 个空格）

2. 重要地方（或者非常规思路）必须添加注释，不限于 JavaScript，CSS 也可以注释

所有前端相关文件类型统一使用 `Prettier` 插件进行格式化，一共修改以下五处配置：

1. 箭头函数
    ![xeWZv9.png](https://s1.ax1x.com/2022/09/28/xeWZv9.png)

2. 每行代码长度
    ![xeWh5T.png](https://s1.ax1x.com/2022/09/28/xeWh5T.png)

3. 去除分号
    ![xeWbrR.png](https://s1.ax1x.com/2022/09/28/xeWbrR.png)

4. 缩进空格数
    ![xeWXa6.png](https://s1.ax1x.com/2022/09/28/xeWXa6.png)

5. 末尾逗号
    ![xefpxH.png](https://s1.ax1x.com/2022/09/28/xefpxH.png)

## JavaScript

1. 字符串使用双引号

2. 代码末尾不加分号

3. 禁止一行代码以 `(` 或者 `[` 开头（会被 JavaScript 认为方法调用或者是数组元素）

4. 重要自定义函数（方法）必须进行注释
    - 函数必须标注用途
    - 形参必须标注含义
    - 形参必须标注类型（如果使用 TypeScript 可以不标注）

5. 禁止匿名函数自调用，如 `(() => {})()` 的形式

6. 禁止使用 `var`，少用 `let`，多用 `const`，非必要情况，不使用 `let`

7. 添加定时器要进行清理，UI 框架中必须清理生命周期中的定时器

8. 对于已知类型却为空的变量使用 `null`，未知类型为空的变量使用 `undefined`

9. 变量命名必须使用小驼峰命名，且能顾名思义，常量命名必须全部大写

10. 禁止使用 `==` 判断相等，必须使用 `===` 判断相等

11. 少用 `for` 循环，多用数组的高级方法代替

12. 少用多层 `for` 嵌套，避免死循环

13. 少用 `else if`，少用 `if` 嵌套，尽量在 `if` 语句执行后，使用 `return`、 `break` 或者 `continue` 跳出判断的链条

## TypeScript

1. 代码末尾不加分号

2. 尽量少用 `any`，非必要情况，不使用 `any`

3. 对象类型声明优先使用 `interface`，其次使用 `type`

4. 类型别名必须使用大驼峰命名

## CSS

1. 必须使用 less（less 是 css 的超集，全部使用 css 写法也可以），了解 less 的基本用法

2. `id`、`class` 等必须使用 `header-logo` 的语义化形式

3. 尺寸大小尽量使用偶数，非必要情况，不使用奇数

4. 字体大小尽量设置为 4 的倍数，如 `16px`，`20px`，非必要情况，不使用奇数

5. 边距大小尽量设置为 8 的倍数，如 `8px`，非必要情况，不使用奇数

6. 盒子模型必须使用 `border-box`，全局定义 `* { box-sizing: border-box; }`

7. 尽量使用 `flex` 布局实现，非必要情况，不使用 `float`

## Vue

1. Vue 文件中三个标签的顺序必须是 `<script>`、`<template>`、`<style>`

2. Vue 组件文件名必须使用大驼峰命名法

3. Vue 必须使用组合式 api （简化代码，避免 `this` 指向问题）

4. Vue 的基础技术栈为 `Vite` + `Vue3` + `Vue Router` + `Pinia`

5. 事件绑定禁止直接写函数体，必须使用箭头函数进行包裹，比如 `@click="dosomething(data)"` 必须改写成 `@click="() => dosomething(data)"`

6. 禁止使用 `v-html`
