# [vue-code-diff](https://www.npmjs.com/package/vue-code-diff)

> 代码比对展示 [demo](http://diff.xjie.me/)

## 安装
```shell
yarn add vue-code-diff
```

## 使用
```vue
<template>
  <div>
    <code-diff :old-string="oldStr" :new-string="newStr" :context="10" />
  </div>
</template>

import vueCodeDiff from 'vue-code-diff'
export default {
  components: {vueCodeDiff},
  data(){
    return {
      oldStr: 'old code',
      newStr: 'new code'
    }
  }
}
```

## 参数说明

| 参数      | 说明    | 类型      | 可选值       | 默认值   |
|---------- |-------- |---------- |-------------  |-------- |
| old-string| 陈旧的字符串| string  |   —    |    —     |
| new-string| 新的字符串| string  |   —    |    —     |
| context| 不同地方上下间隔多少行不隐藏 | number  |   —    |    —     |
| outputFormat| 展示的方式 | string  |   line-by-line，side-by-side    |    line-by-line     |


## 效果展示

### line-by-line
![image](https://github.com/ddchef/vue-code-diff/blob/master/2018-06-01.png?raw=true)

### side-by-side
![image](https://github.com/ddchef/vue-code-diff/blob/master/2018050615272.png?raw=true)

## LICENSE
[MIT](LICENSE)
