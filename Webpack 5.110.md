# Webpack 5.110

_12 Sep 2026_

> [!IMPORTANT]
> Если в системе установлен только Bun (без Node.js и npm), тогда лучше создать символьные ссылки, т.к. create-webpack-app требует npm.

```bash
ln -s $(which bun) $(dirname $(which bun))/node
ln -s $(which bun) $(dirname $(which bun))/npm
```

## 1. Get Started

```bash
bunx create-webpack-app my-webpack-app --template react
# TypeScript / React State - yes / PWA - no / CSS - none / npm

cd my-webpack-app
bun run build
bun serve
# Вместо `bun serve` можно запустить`bun ./dist/index.html`
```

ℹ️ Размер JS-бандла: 183 kB

Ссылки

1. [Webpack site](https://webpack.js.org/)
2. [Webpack GitHub](https://github.com/webpack/webpack) ⭐ 65.9k
3. 👉 [Getting Started](https://webpack.js.org/guides/getting-started/)
4. [create-webpack-app](https://github.com/webpack/webpack-cli/tree/main/packages/create-webpack-app)
