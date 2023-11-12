# fengmao-ui

## [Vue2 基于 Element-ui 基础组件传送门]

> 基于 Element-ui 二次封装基础组件地址

> 基于 ant-design-vue 二次封装基础组件地址(期待中)

## 介绍

> 基于 vue3+ ts+ Element-plus 二次封装组件

这是我在学习 Vue3 中基于[Element-plus](https://element-plus.org/zh-CN/) 二次封装基础组件文档，希望对你有用。Table 组件使用方式：

## npm 方式安装使用

```shell
npm i fengmao-ui
```

## 全局注册使用

> ### 前提条件：使用项目必须全局注册 Element-plus 组件库

```js
// 在main.js中按下引入
import fengmaoUi from 'fengmao-ui'
import 'fengmao-ui/lib/style.css'
Vue.use(fengmaoUi)
```

## 按需引入

```js
// 在main.js中按下引入
import 'fengmao-ui/lib/style.css'
// 单个.vue文件引入
;<script setup lang="ts">
  import {(TDetail, TForm)} from "fengmao-ui"
</script>
```

## fengmao-ui Volar 组件类型提示

```js
// 需要在使用的项目的tsconfig.json文件中添加以下
compilerOptions：{
  "types": [
      "fengmao-ui/components.d.ts",
    ],
}

```

## Vue3 + Vite 项目中安装引入报如下错误的解决方法

> #### 把项目的 vite 版本升级到 4+

<img src="./README_GIF/error.png">

## 安装依赖

> ### 注意: 本地环境版本最好安装 [Node.js 16.x+](https://nodejs.org/en)、[pnpm 7.x+](https://github.com/pnpm/pnpm/)

```shell
npm install -g pnpm

pnpm install

```

## Git 提交规范

- `ci`: ci 配置文件和脚本的变动;
- `chore`: 构建系统或辅助工具的变动;
- `fix`: 代码 BUG 修复;
- `feat`: 新功能;
- `perf`: 性能优化和提升;
- `refactor`: 仅仅是代码变动，既不是修复 BUG 也不是引入新功能;
- `style`: 代码格式调整，可能是空格、分号、缩进等等;
- `docs`: 文档变动;
- `test`: 补充缺失的测试用例或者修正现有的测试用例;
- `revert`: 回滚操作;
