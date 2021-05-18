# 第一次使用nuxt制作网站

# nuxt-text

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

全局安装create-nuxt-app

```bash
npm install -g create-nuxt-app
```

创建(项目名不能有大写字母)

```bash
npx create-nuxt-app 项目名/yarn create nuxt-app 项目名
```

### 路由

路由传参

```vue
<nuxt-link :to="{name:'about',query:{id:456}}">about</nuxt-link>
<nuxt-link :to="{name:'news',params:{xid:123}}">news</nuxt-link>
```

接受参数

```vue
<h2>接收到route.query为{{$route.query.id}}</h2>
<h2>得到的xid是{{$route.params.xid}}</h2>
```

动态路由

在pages页的news文件夹中原本结构为/news/index.vue

现在创建一个新的文件_id.vue在news目录中，然后使用动态路由传参

```html
<a href="/news/4567">动态路由</a>
```

接受参数

```vue
//_id.vue
<h2>得到的xid是{{ $route.params.id }}</h2>

//script
export default {
  validate({params}) {
      console.log(params)
      return params.id === '4567'
  },
};
```

