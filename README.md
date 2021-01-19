# xconfigurator.github.io.vuepress

## 参考
[https://vuepress.vuejs.org/zh/guide/getting-started.html](https://vuepress.vuejs.org/zh/guide/getting-started.html)
[https://24kcs.github.io/vue3_study/chapter7/%E5%BF%AB%E9%80%9F%E6%90%AD%E5%BB%BA%E5%9C%A8%E7%BA%BF%E6%96%87%E6%A1%A3.html#_2-%E9%85%8D%E7%BD%AEts%E6%95%99%E7%A8%8B%E6%96%87%E6%A1%A3](https://24kcs.github.io/vue3_study/chapter7/%E5%BF%AB%E9%80%9F%E6%90%AD%E5%BB%BA%E5%9C%A8%E7%BA%BF%E6%96%87%E6%A1%A3.html#_2-%E9%85%8D%E7%BD%AEts%E6%95%99%E7%A8%8B%E6%96%87%E6%A1%A3)

## 初始化
```shell
# 基本
git clone git@github.com:xconfigurator/xconfigurator.github.io.vuepress.git
yarn init # npm init
yarn add -D vuepress # npm install -D vuepress

mkdir docs && echo '# Hello VuePress' > docs/README.md

# 为发布到github pages的工具
yarn add -D gh-pages
```

## 添加配置并启动 (package.json)
```json
{
  "scripts": {
    "docs:dev": "vuepress dev docs",
    "docs:build": "vuepress build docs",
    "docs:deploy": "gh-pages -d docs/dist"
  }
}
```

## 在本地启动服务器
```shell
yarn docs:dev # npm run docs:dev
```

## 发布到github pages
```shell
yarn docs:build
yarn docs:deploy
```