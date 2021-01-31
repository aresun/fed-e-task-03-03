# nuxt

## 文件结构

- `pages/`
  - 存放根路径下的页面, 在地址栏通过文件名访问
  - 前端路由, 由文件结构自动生成
- `.nuxt`
  - `nuxt` 编译后的 `client` 与 `server`

## route

- 会刷新页面, 请求 server render
  - `<a herf="/">index page</a>`
- 前端路由导航
  - `<router-line to="/"></router-line>`
  - `this.$router.push('/')`
- dynamic router
  - use `_id.vue` to match `id` page
  - `$route.params.id` to get param inside url path
- child router export
  - `<nuxt-child />`

## `src/app.html`

- replace default html root template
- `{{APP}}` page content will be replaced here

## `layouts/default.vue`

- 路由外层页面
- 在 component 里添加 layout: `layout: 'layout_name'`

## asynchronous data

- `static/data.json`; default mock data
- `asyncData`
  - no `this` in this function 
  - only for pages component
  - 调用时机:
    - server render
    - before client routing
  - `context` arg in `asyncData`
