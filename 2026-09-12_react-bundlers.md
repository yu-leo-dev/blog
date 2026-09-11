## Исследуем сборщики для React

### 1. [Webpack 1.110](https://webpack.js.org/)

См. [create-webpack-app](https://github.com/webpack/webpack-cli/tree/main/packages/create-webpack-app)

```bash
mkdir my-webpack-app && cd my-webpack-app
bunx create-webpack-app --template react # TypeScript / React State - yes / PWA - no / CSS - none / npm
rm -rf node_modules  package-lock.json
bun i
bun run build
bun ./dist/index.html
```
ℹ️ Размер JS-бандла: 183 kB
