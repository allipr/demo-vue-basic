# Vue3.0 OptionsAPI

> Vue3.0选项式API

## （一）基础

### data()

### methods

### computed

### watch

### Lifecycle Hooks

#### 生命周期事件

| 选项式 API        | Hook inside `setup` | 含义     |
| ----------------- | ------------------- | -------- |
| `beforeCreate`    | Not needed*         | 创建前   |
| `created`         | Not needed*         | 创建后   |
| `beforeMount`     | `onBeforeMount`     | 挂载前   |
| `mounted`         | `onMounted`         | 挂载后   |
| `beforeUpdate`    | `onBeforeUpdate`    | 更新前   |
| `updated`         | `onUpdated`         | 更新后   |
| `beforeUnmount`   | `onBeforeUnmount`   | 卸载前   |
| `unmounted`       | `onUnmounted`       | 卸载后   |
| `errorCaptured`   | `onErrorCaptured`   | 错误捕获 |
| `renderTracked`   | `onRenderTracked`   | 渲染跟踪 |
| `renderTriggered` | `onRenderTriggered` | 渲染触发 |

#### 生命周期图示

![实例的生命周期](01-optionsAPI.assets/lifecycle.svg)

#### 示例

```js
Vue.createApp({
  data() {
    return { count: 1}
  },
  created() {
    // `this` 指向 vm 实例
    console.log('count is: ' + this.count) // => "count is: 1"
  }
})
```



## （二）升级
