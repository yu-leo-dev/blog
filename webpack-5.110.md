# Webpack 5.110

_12 Sep 2026_

## 1. Get Started

> [!IMPORTANT]
> Если в системе установлен только Bun (без Node.js и npm), тогда лучше создать символьные ссылки, т.к. create-webpack-app требует npm.

```bash
ln -s $(which bun) $(dirname $(which bun))/node
ln -s $(which bun) $(dirname $(which bun))/npm
```

```bash
bunx create-webpack-app my-webpack-app --template react
# TypeScript / React State - yes / PWA - no / CSS - none / npm

cd my-webpack-app
bun run build
bun serve
# Вместо `bun serve` можно запустить bun ./dist/index.html
```

> [!NOTE]
> 📦 Размер основного JS-бандла: 183 kB (react-dom 132kB, react-router-dom 41kB, react 8kB)
> ⚠️ Если апгрейдится до React 19.3, то бандл будет 262kB [+79kB] (react-dom@19.3 210kB)

Ссылки

1. [Webpack site](https://webpack.js.org/)
2. [Webpack GitHub](https://github.com/webpack/webpack) ⭐ 65.9k
3. 👉 [Getting Started](https://webpack.js.org/guides/getting-started/)
4. [create-webpack-app](https://github.com/webpack/webpack-cli/tree/main/packages/create-webpack-app)
