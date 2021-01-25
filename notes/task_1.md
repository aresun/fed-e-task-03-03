# vuex

## 简化方法

- `mapState`
- `mapGetter`
  - Getter 就是 store 中的计算属性，使用 mapGetter 简化视图中的使用
- `mapMutations`
  - 更改 Vuex 的 store 中的状态的唯一方法是提交 mutation
- `mapActions`
  - Action 提交的是 mutation，而不是直接变更状态
  - Action 可以包含任意异步操作
- `Module`
  - 每个模块拥有自己的 state、 mutation、action、getter、甚至是嵌套子模块
